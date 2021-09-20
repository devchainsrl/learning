# Workshop - GIT
---

This workshop covers the basic git commands.

> For more materials check the [workshop extras page](../extra/README.md)

## Introduction

#### What is GIT? 

Git is a version control system (VCS) for tracking changes in computer files and coordinating work on those files among multiple people. 
It is primarily used for source code management in software development, but it can be used to keep track of changes in any set of files. 

As a distributed revision control system it is aimed at speed, data integrity, and support for distributed, non-linear workflows.


### Terminology

#### Data Structures
* A `blob` (binary large object) is the content of a file. Blobs have no proper file name, time stamps, or other metadata. (A blob's name internally is a hash of its content.)
* A `tree` object is the equivalent of a directory. It contains a list of file names, each with some type bits and a reference to a blob 
or tree object that is that file, symbolic link, or directory's contents. 
  * These objects are a snapshot of the source tree. 
(In whole, this comprises a Merkle Tree, meaning that only a single hash for the root tree is sufficient and actually used in commits to
exactly pinpoint to the exact state of whole tree structures of any number of sub-directories and files.)
* A `commit` object links tree objects together into a history. It contains the name of a tree object (of the top-level source directory), a time stamp, a log message, and the names of zero or more parent commit objects.
* A `tag` object is a container that contains a reference to another object and can hold added meta-data related to another object. Most commonly, it is used to store a digital signature of a commit object corresponding to a particular release of the data being tracked by Git.

#### References
* `heads` refers to an object locally
* `remotes` refers to an object which exists in a remote repository
* `stash` refers to an object not yet committed
* `meta` - e.g. a configuration in a bare repository, user rights;
* `tags` - see above


Sources:
[Git - Wikipedia](https://en.wikipedia.org/wiki/Git)


### [Git Commands](git-commands.md)
### [Step 1](step-1.md)