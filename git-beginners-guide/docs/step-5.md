# Workshop - GIT
---

### [Previous: Step 4](step-4.md)

## Step 5: Teamwork 2 - Common Issues

This step covers the basics of working with branches.

### Working on out-of-date commit

It often happens to developers to work simultanously on the same branch.

Even if not working on the same file both developers must pull the changes locally before continuing.

Other cases:
* When new commits are pushed to a base branch and the derived branch remains outdated
* When working

> Note: all new php files will be added inside the `src` directory

### Tasks to reproduce (same branch):
* Create two PHP files: `d.php` and `e.php`
* Add some code in both files
* Commit and push changes
* Change some code in `d.php`
* Commit and push changes
* Reset to a commit earlier (`HEAD^`)
* Change some code in `e.php`
* Commit changes
* Try pushing changes

### Tasks to reproduce (different branches):
* Switch to `master` branch (if not already switched)
* Create two PHP files: `d.php` and `e.php`
* Add some code in both files
* Commit and push changes
* Copy `master` branch to a new one, name it `new-feature-2`
* Change some code in `d.php`
* Commit and push changes 
* Switch branch to `master`
* Change code in `e.php`
* Commit and push changes

### [Next: Extra](extra.md)

### [Git Commands](git-commands.md)
### [Main Page](README.md)
