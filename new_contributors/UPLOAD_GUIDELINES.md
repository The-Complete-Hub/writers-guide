## How to upload an article for The Complete Hub

**Prerequisites:**
- Github account
- Text editor, such as [Visual Studio Code](https://code.visualstudio.com/), [Sublime Text](https://www.sublimetext.com/), [Atom](https://atom.io/)
- Prepared markdown (.md) file. (Note: All articles must be submitted in properly-formatted markdown). See [Github Markdown guide](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

### Fork the repository
In order to upload your prepared .md file to Github, first, click the **Fork** option in the upper right-hand corner (pictured below).

![Fork Image](images/fork_repo.png)

Once you have successfully forked over to your repository:
- You should notice your username in the upper left-hand corner (top red arrow).
- If a Github Action notice pops up, click **Dismiss** (red arrow in the middle).

General rules:
Always make changes to your main branch.


Always keep ur fork up to date with The-Complete-Hub/writers-program

### Clone the forked repository
Next, you will need to clone the repository to your local computer.

![clone repository](images/clone-image.png)

Open the newly cloned repository in your text editor. It should look something like this (shown in Visual Studio Code):

![repository text editor](/images/vs_code.png)

Note: When working with multiple articles simultaneously, it's best to create and work on separate branches for each article. (Here is a [short video](https://www.youtube.com/watch?v=oPpnCh7InLY&t=577s) on how Github Branches work.)

### Create article folder structure
Within the articles folder (inside the content folder), create a new folder using the intended url for the article. (Reference existing folders' naming conventions.)

Be sure to:
- **Use all lowercase.**
- **Use dashes in place of spaces.**
- **Do not include any special characters.**
- **Try to keep it under 40 characters.**
- -**Avoid using periods (.) or commas (,) or (_ ) underscores**

![create article folder](/images/folder_structure.png)

Within that article folder, upload your prepared .md file containing article contents using the filename `index.md`. Upload any corresponding image files referenced in your article. When referencing images, be sure to use the following naming convention with your newly created article directory.

For example:

`![image title](/new-folder-name/image-name.jpg)`

If you have a header (hero) image in mind, feel free to include it your PR as well. Please try to keep images as close to **600X400 pixels** (images can be resized using [Pixlr Image Editor](https://pixlr.com/e)) and make sure you have the appropriate copyright to use it. Sites like [Unsplash](https://unsplash.com) have Creative Commons images which you can use for free.

Any images within the article need to be hosted on our site - (place the image in the proper folder) - and have the proper image paths in the article similar to the hero image and have citations (attribution) if required.

Your folder should now look similar to this:

![folder contents](images/article_image.png)

Once your files are properly uploaded and organized, add, commit, and push your changes to your forked remote Github repository either using the command line or the Github tools within your text editor.

### Create pull request
Open Github. You should see a message indicating your pushed changes with a button to 'Compare & pull request'.

Open a pull request that includes the name of your article and a description of the contents that you are submitting.

***Note***: Make sure your repository is up to date with The Complete Hub Writers Program Repo before contributing new articles.

### do this once
`git remote add section https://github.com/The-Complete-Hub/writers-program`

### then use this every time before contributing a new article to keep it up to date

```bash
git fetch section
git pull --rebase section master
git push origin
```

Finally, make sure you take advantage of this useful tool, [Hemingway](http://www.hemingwayapp.com) that helps with word count, formatting, and grammar/readability.

By highlighting lengthy, complex sentences and common errors, it helps make any writing BOLD & CLEAR. If you see a yellow sentence, you may want to shorten or split it. Please use on all future articles before submitting a PR (pull request).

To review your Code Snippets or examples before submitting, take full advantage of the free online tool, [repl.it](https://repl.it). Use it to run and compile any code snippets to be included in your article.

### Including videos in your articles
If you would like to include a (step-by-step) video to one of your How To Guide or Tutorial videos feel free to do so as a YouTube iframe.

Follow the steps, stated below:

1. Upload the video to YouTube, if it isn't already.

![Copy YouTube Embed Code](images/youtube embed.png)

Take that copied embed code and paste it into your .md (markdown) file where you would like it to be placed. The code should look something like this:

`<iframe width="956" height="538" src="https://www.youtube.com/embed/npnp--SSx_8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>`

*NOTE:* If the width and height are not `width="478" height="269"` be sure to change the sizes to fit our web page format.

Following duly every step and guideline stated here, your article should be ready to be published right now. Send in a PR and we will be glad to approve and upload your article on TC Hub site.
