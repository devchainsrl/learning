# Workshop - GIT
---

### [Previous: Step 1](step-1.md)

## Step 2: Adding files

In this step you will add some files into your project and commit them.

### Tasks:

* Add some files to the project
* Create a directory named `src` and add a php file
* Create a directory named `extra` to add other kinds of files (for now)
* Commit the files

> Note: PHP files must comply to PSR-2 coding standard 

#### Are the files published?

At this point the files are commited on your machine, but not published.

The commit can be ammended, therefore if you made a mistake you can either amend the commit or perform a [`soft reset`](https://git-scm.com/docs/git-reset).

If you want to add or remove files the following must be done:

`git reset HEAD~` - to reset to previous commit
`git add .` - to add all changed files
`git commit -m "commit message"` - to commit the files

### [Next: Step 3](step-3.md)

### [Git Commands](git-commands.md)
### [Main Page](README.md)
