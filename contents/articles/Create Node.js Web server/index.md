---
slug: Create-a-Node.js-web-server-with-Express-Framework
title: Create a Node.js web server with Express Framework
author: [Jesse Oluwadare]
tags: [Node.js, Backend development, express, Web server]
---

# Introduction
Node.js is a javascript framework that allows us to run javascript outside the browser, it is a javascript runtime built on chrome v8 engine.

Skipping the not-so-boring stuff we will be trying our hands at building a simple web server using a popular javascript framework called 'Express'. Express is a framework that gives node.js superpowers because of its amazing feature. Express is built on top of Node's features to provide easy to use functionality, it runs between the server created by Node.js and the frontend pages of our application.

**Let us dive in 👨‍💻!**

So what is a web server? A web server in simple terms hosts our web pages and web content. To access these contents clients (i.e browsers) make an HTTP request to the server for these contents.

# Developer Environment setup

To follow through with this tutorial you would have to install Node and you can do this by going to the official [Node site](https://nodejs.org/en/). If Node is already installed you can check your node version by opening your command prompt and typing `node -v` . If Node.js is installed the version installed will be displayed.

Since Node.js is installed, we need to create a directory for the project using the `command mk-dir project-name` (project-name is the name of your directory) you can navigate to the directory with the command `cd project-name`. To start our project and create a package.json file, we run the command `npm init`. A package.json file contains basic information about your project such as the name, author, version, description and dependencies ...we won't be diving into all of that in this article.

...for starters

> **npm [(Node Package Manager)](npmjs.com)** is a package manager for the JavaScript programming language maintained by npm, Inc. npm is the default package manager for the JavaScript runtime environment Node.js. It consists of an online database of public and paid-for private packages, called the npm registry. It is a command-line tool used to share Node.js packages/modules.

To install a package in this project, navigate to your desired directory and run `npm install package-name` on the terminal. to install a package globally, run `npm install package-name --global` (shortcut -g instead of --global). We need to install Express in this project's directory, we'll run the command `npm install express --save`. also for --save (shortcut -s) now our package is added to the list of dependencies in the package.json file.

Now we are done with the setup, we can now go to building our server.

# Code along

Navigate to your code editor and create an index.js file in the directory created earlier.

Now, we have to import the installed express module.

```javascript
const express = require("express");

// Now we have to create an instance of express
const app = express();

// we tell `app` to listen for GET requests to our server based on the specified path ('/') and send a specific response, using the get() method:
app.get("/", (req, res) => res.send("My Node.js Web Server 🐱‍🏍!"));



// we start our web server by telling the app to listen on a specific port (8000 in this case) and run our callback function when the server starts up:
app.listen(8000,  () =>
console.log("Listening to port 8000 successful!")
```

# Starting the Server

Inorder to run the code that we have just written and start up the server, we simply run `node index.js` in our terminal, shortcut to open terminal in vs Code`ctrl + Shift + ` ` , then open localhost:8000 in your browser. You should see the response displayed.

# Conclusion:

Hope you had fun building this simple web server with express. I hope you keep on learning and building more amazing projects. There will be more articles surrounding web development topics.
