# Workshop - GIT
---

### [Previous: Step 3](step-3.md)

## Step 4: Teamwork 1 - Branches

This step covers the basics of working with branches.

In the first phase some files will be added.

### Tasks:
* Create two PHP files: `a.php` and `b.php` inside the `src` directory
* Add some code in both files (the code won't be executed)
* Commit and push your changes to `origin/master`

When a new feature must be implemented and we don't want to affect other developers working on the project the best option is to create a new branch.

After finishing working on our new feature the branch can be merged in to the master branch.

### Tasks:
* Create a new branch, name it `new-feature`
* Add another PHP file named `c.php` inside the `src` directory
* Add some code in `src/b.php`
* Commit and push the changes to `origin/new-feature`
* Add another file in the `extras` directory (assuming it's a file needed for the new feature)
* Merge the the branches so all content will be in `origin/master` (don't forget to commit and push the previous changes!)

> Note: The branch will be created on the git server only when pushing the commits


### [Next: Step 5](step-5.md)

### [Git Commands](git-commands.md)
### [Main Page](README.md)
