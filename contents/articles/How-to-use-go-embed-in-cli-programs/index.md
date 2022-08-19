---
slug: embedding-static-files-in-cli-with-go-embed
title: Embedding templates and static files in CLI using //go:embed
author: Saintmalik
author_title: Pentester
tags: [Golang, Go, CLI, static files]
---

or someone who just started writing Go, i have no idea about //go:embed feature which came with the released version: 1.16.

A project i was working on recently led to the discoveries.

<!--truncate-->

## So what is //go:embed?

The embed package allows us to embed static/template or directories into our Go program

## When should you use //go:embed in your project?
//go:embed can be used in situations where the file or assets won't change or be modified after build, dont shoot yourself in the leg by embedding files that are subjected to modifications e.g ```config.json``` and all type of files similar to this

examples of assets that you can use ```//go:embed``` for are ```templates/css``` files and anything similar to this

## How to use it in CLI programs?

If you are writing your CLI tool using frameworks like cobra, urfave-cli, you will know that your commands files e.g root.go and the likes are alway in a "cmd" folder

```mdx
hello_cobra
├─ cmd
│  ├─ config.go
│  ├─ root.go
│  └─ run.go
├─ go.mod
├─ go.sum
├─ main.go
└─ templates
   ├─ config.html
   ├─ creds.html
   └─ index.html
```

and the rule that comes with //go:embed is that you can only embed via your root folder, so lets say you have your template folder inside your main project folder, just the way my project folder is above

Then you can easily embed using main.go file in your root folder or any other go file in root folder

but in situation where your template files is needed or called inside your "cmd" folder, i need to embed my template from my cmd>>config.go file.

It becomes tricky from there? you get it right? meaning  //go:embed won't work, it will start spitting errors like ```pattern ****/: no matching files found```

because you can only use embed from the root files and now you need to call it from a file inside the "cmd" which is not available on the root.

i was stucked man, spent two to three days thinking and searching the internet for solution, pushing my project depends on getting the static/template assets files embed.

Now you probably thinking why dont i move my template folder into the "cmd" folder? yes i did that too, but using   ```//go:embed templates/*.html``` wasnt working still

but at last i stumbled upon https://github.com/plentico/plenti repo, the guy did what i have been trying to do, infact he has lot of static files

but what he did is different from what every article i have come acrossed did and shared, he used this syntax ```//go:embed all:yourfolders/*``` while other content out there states to use this ```//go:embed yourfolders/*```

don't get me wrong both ar correct, but ```//go:embed all:yourfolders/*```  works well for embedding from files that are not in root folder, in situations where your folder is like this

```mdx
hello_cobra
├─ cmd
│  ├─ config.go
│  ├─ root.go
│  └─ run.go
└─ templates
   ├─ config.html
   ├─ creds.html
   └─ index.html
├─ go.mod
├─ go.sum
├─ main.go
```

and how is i embedthe templates in my config.go

```go title="hello_cobra/cmd/config.go"
package cmd

import (
	"embed"
	"fmt"
	"net/http"
	"text/template"

	"github.com/spf13/cobra"
)

//go:embed all:templates/*.html   //this means, embed all files ending with ".html"  in the templates folder even when ignored
var TempFs embed.FS //assign the variable TempFs to embed.FS, FS means (File System)

var tmpl *template.Template //tmpl is a type pointer to template.Template,


func init() {
	rootCmd.AddCommand(configCmd)
	tmpl = template.Must(template.ParseFS(TempFs, "templates/*.html"))
}

func myTempl(w http.ResponseWriter, _ *http.Request) {

///you can do all your codes here,
	err = tmpl.ExecuteTemplate(w, "creds.html", nil) //Executing the template
	if err != nil {
		log.Fatal("Error loading index template: ", err) //log an error, if the template cant be started
	}
}
```

And that's all, If you want to learn more about //go:embed read over here <a href="https://pkg.go.dev/embed">here</a>.