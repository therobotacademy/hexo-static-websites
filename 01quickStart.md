# 1. Quick start
https://www.cgmartin.com/2016/01/03/getting-started-with-hexo-blog/
```
$ sudo npm install -g hexo-cli
$ hexo init blog && cd blog
$ npm install
```
## Start the server
```
$ hexo server --draft --open
   INFO  Start processing
   INFO  Hexo is running at http://localhost:4000 . Press Ctrl+C to stop.
```

This starts the server with a few extra options:

 - `--draft` : Enables viewable "draft" posts (by default, drafts are hidden)
 - `--open` : Open the local site in your browser

 You'll want to leave the server running in the terminal while authoring. The server process will watch for changes made to the Markdown source files and automatically generate new HTML files. The server's console log output is also helpful for troubleshooting errors that you may run across.

## Create the first post
```
$ hexo new draft "My First Blog Post"
# creates -> ./source/_drafts/My-First-Blog-Post.md
```
Other templates besides "draft" can be used when using the hexo new command. Look under the ./scaffolds/ folder and read the [Hexo documentation on Scaffolds](https://hexo.io/docs/writing.html#Scaffolds) for more information.

To edit your draft, navigate to `./source/_drafts/My-First-Blog-Post.md` and open the file with your favorite Markdown editor.
```
---
title: My First Blog Post
tags:
---
## Hello there
This is some content.
```

The stuff between the dashes --- at the top of the markdown file is called "front-matter". It is metadata that is used by Hexo and the active theme. See the Hexo documentation on Front-Matter for more information.

Saving changes to your Markdown files will be automatically detected by the running hexo server and regenerated as static HTML files, but you must refresh the browser to view the changes.

## Automatic refresh of pages
If you dislike having to manually refresh the browser each time, the hexo-livereload or hexo-browsersync plugins can do it automatically.

To install the hexo-browsersync plugin (my personal favorite):
```
$ npm install hexo-browsersync --save
$ hexo server --draft --open  # restart the server
```
Hexo website runs again at  `http://localhost:4000`
Browser sync settings runs at `http://localhost:3001`

## Displaying summary excerpts in listings

## Inserting images

## Publishing drafts

## Next steps

## Getting help
