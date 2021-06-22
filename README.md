# setpaths-cli
A CLI command to set up a folder structure for development.

This will create a development folder structure in ${your_home_directory}/Documents/dev

## How to
```
 1. sudo npm i -g @hakansundstrom/setpaths-cli
 2. run 'setpaths createfolders' from your terminal.
 3. Copy the generated aliases into your .zshrc or .bashrc file via a texteditor via 'nano ~/.zshrc' or 'vim ~/.zshrc'*
 4. Save to file. (Read about 'nano' or 'vim' editor if you dont know how to write to file.) nano is the most beginner friendly.
 4. Done! Write something like 'p.dev' or 'p.sandbox' or 'p.node' to terminal, all paths have these shortcuts now.
```

Step 3 explanation. Depending on your shell, this should either be pasted via `nano ~/.zshrc` or `nano ~/.bashrc`, here I use nano text editor for simplicity. Write `echo "$SHELL"` to your terminal to see what shell you're using. If output is something like `/bin/zsh` you are using zsh and same goes for bash and other shells.

All paths are accesible from terminal via 'p.{folderName}'.
The terminal will also display what folders and files are in there.

You can also fork this from github to a custom folder.

Execute this by entering 'node ${path-to-this-folder}/setpaths'. 

Customise your folder structure and paths in the fullPaths object as you'd like.

## The generated folder structure tree will look like this
````
 Folder structure:
 dev
   bin # Executables
   production # Live projects
   debugging
   showcase # Showcase your skills repos
   work # Your work related repos
   docs # Random dev. specific documents
   sandbox # Just for learning and playing around
     git
     docker
     desktop
     mobile
     web
       frontend
       backend
       fullstack
     rdm # (Random)
       github # Random specific github repos
     langs # Practice/play with different programming languages
       c
       c++
       c#
       java
       python
         python3
       node
       objective-c
       swift
       assembly
       javascript
       typescript
       php
````

## Requirements:
Node
MacOS or Linux
