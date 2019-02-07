---
layout: post
title: Typical Git Commands
---

This guide will help you as you get started with git.  It doesn't cover all the details, but it also doesn't surround you with detail you won't use.

## Typical Workflow
  1. Get all code (clone)
  2. Switch to a starting branch (checkout)
  3. Create your own branch (checkout)
  4. Add new files / Make changes to files
  5. Stage all your changes (add)
  6. Commit your changes (commit)
  7. Push your changes
  
  Sometimes you will repeat steps 4,5,6 several times.  In which case you might want to squash your changes (will be explained later)

## Commands
`git clone <repo url>`
`cd repo name`
`git checkout develop`
`git checkout -b branch-name`
`git add mynewfile.js`
`git add existingfile.js`
`git commit -m "Added new file, modified exssitng file"`
`git push origin branch-name branch-name`

## Detailed Explanations of the above
1. `git clone <repo url>`
This command will download the repository and it's history on to your local machine.  
**Sample:** 
`git clone git@github.com:SameerDoshi/gittutorial.git`

2. `cd repo name`
This simply moves to the directory that was created
**Sample:** cd gittutorial

3. `git checkout develop`
Typically you will not be allowed to make changes directly to the master branch.  But instead will have to make changes to the develop branch.   Others may have changes in develop that are not yet in master.  You should start with develop.  This command changes your branch to develop.
**Sample:** git checkout develop

4. `git checkout -b branch-name`
Now you'll create a custom branch name that will track all of your work.  Branch names are case sensitve and I reccomend you do not use spaces.
**Sample:** git checkout -b adding-index

5.`git add mynewfile.js`
After creating (or modifying) files you need to add them to the staging area.  To do this use the add command.
**Sample:** git add index.html

6. `git commit -m "Added new file, modified exssitng file"`
When you're finished adding all your files you'll commit and include a commit message.  If you don't use `-m "a sample message"` then you'll be promotped to enter a message.
**Sample:** git commit -m "Initial commit"

7. `git push origin branch
This command pushes your branch to the server
**Sample:** git push origin adding-index


### Additional Help
The GitHub [HelloWrold project](https://guides.github.com/activities/hello-world/)  provides details for how the entire workflow above. 
