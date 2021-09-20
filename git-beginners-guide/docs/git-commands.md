# Workshop - GIT
---

## GIT Commands

### Repository creation

Create a new local repository

`$ git init` 

Clone an existing repository

`$ git clone ssh://user@domain.com/repo.git`

or using http

`$ git clone http://user@git.domain.com/repo.git`


### Local changes

* Display changed files in your working directory

`$ git status`

* Add a file to tracking

`$ git add <filename>`

* Add multiple files to tracking

`$ git add <filename> <filename2> ... <filenameX>`

* Add files from a directory to tracking

`$ git add <dirname>` 

> Note: an empty directory cannot be tracked, git only tracks files

* Add all current changes to the next commit

`$ git add .`

> Note: `git add .` actually adds the current folder's content

> Command must be ran in the project's root directory, otherwise only the files in current directory will be added

> Find current directory with `pwd` (linux) or `cd` (windows)


* Add some changes in <file> to the next commit

`$ git add -p <file>`


* View changes to tracked files

`$ git diff`


* Commit all local changes in tracked files

`$ git commit -a`

* Commit previously staged changes

`$ git commit`

* Change the last commit

`$ git commit --amend`

> Don‘t amend published commits!

### Commit history

* Show all commits, starting with newest

`$ git log`

* Show changes over time for a specific file

`$ git log -p <file>`


* Display who changed what and when in <file>

`$ git blame <file>`



### Branches and tags

* List all existing branches

`$ git branch -av`

* Switch HEAD branch

`$ git checkout <branch>`

* Create a new branch based on your current HEAD

`$ git branch <new-branch>`

* Create a new tracking branch based on a remote branch

`$ git checkout --track <remote/branch>`

* Delete a local branch

`$ git branch -d <branch>`

* Mark the current commit with a tag

`$ git tag <tag-name>`

### Update & publish

* List all currently configured remotes

`$ git remote -v`


* Show information about a remote

`$ git remote show <remote>`

* Add new remote repository, named <remote>

`$ git remote add <shortname> <url>`

* Download all changes from <remote>, but don‘t integrate into HEAD

`$ git fetch <remote>`

* Download changes and directly merge/integrate into HEAD

`$ git pull <remote> <branch>`

* Publish local changes on a remote

`$ git push <remote> <branch>`

* Delete a branch on the remote

`$ git branch -dr <remote/branch>`

* Publish your tags

`$ git push --tags`

### Merge & rebase

Merge <branch> into your current HEAD

`$ git merge <branch>`

* Rebase your current HEAD onto <branch>

`$ git rebase <branch>`

> Note: Don‘t rebase published commits!

* Abort a rebase

`$ git rebase --abort`

* Continue a rebase after resolving conflicts

`$ git rebase --continue`

* Use your configured merge tool to
solve conflicts

`$ git mergetool`

* Use your editor to manually solve conflicts
and (after resolving) mark file as resolved
`$ git add <resolved-file>`

`$ git rm <resolved-file>`

### Undo

* Discard all local changes in your working
directory

`$ git reset --hard HEAD`

* Discard local changes in a specific file

`$ git checkout HEAD <file>`

* Revert a commit (by producing a new commit
with contrary changes)

`$ git revert <commit>`

* Reset your HEAD pointer to a previous commit
…and discard all changes since then

`$ git reset --hard <commit>`

* …and preserve all changes as unstaged
changes

`$ git reset <commit>`

* …and preserve uncommitted local changes

`$ git reset --keep <commit>`