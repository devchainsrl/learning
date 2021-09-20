# Workshop - GIT
---

### [Previous: Step 2](step-2.md)

## Step 3: Publishing the changes

In this step you will configure the server to which the commited changes will be published.


### Publishing the "changes"

Files cannot published as files, files are published as commits made.

Your local git repository is not currently configured to work online.
In order to publish changes a `git remote` must be configured.

The command for adding a remote is:

`git remote add origin http://github.com/user/repo.git`

> Note: in our case the "username" is `workshop-tests` and the repo is `username-firstproject`, as defined in step 1

To check the newly added remote run:

`git remote -v`

The remote is configured and commits can be published from now on.

To publish your commited changes run the following command:

`git push` - to send/publish your changes to the server (if the remote added)

Optionally the remote and branch can be provided

`git push origin/master`

### Tasks:
* Publish (push) your changes to `origin/master`
* Check if your changes were published VIA the github UI


### [Next: Step 4](step-4.md)

### [Git Commands](git-commands.md)
### [Main Page](README.md)
