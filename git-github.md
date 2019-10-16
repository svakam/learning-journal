# Notes on 'Git Tutorial: A Comprehensive Guide'
https://blog.udemy.com/git-tutorial-a-comprehensive-guide/

## Version control

**Version control:** a system that allows revisiting of different versions of a file or set of files by recording changes. 

Can revert a file or project to previous version/track modifications/modifying individuals/comparing changes

By utilizing a VCS (Version Control System), mistakes can be more efficiently corrected

### Local vs centralized vs distributed VCS

**Local VCS (LVCS):** one database on local hard disk that stores changes to files

**Centralized VCS (CVCS):** single server storing all changes and file versions, which can be accessed by different clients. Eliminated need to involve all local databases and have more active involvement across programmers.  

**Distributed VCS (DVCS):** addresses vulnerability of the CVCS (server as a single point of failure, corruption of central database's hard disk with absence of backups). In place, allows clients to create mlutiple mirrored repos (data backups) which can be placed on the server to replace lost info, and also allows use of different simultaneous workflows. 

**What is Git?** Git is a DVCS that stores data in a file system made of snapshots. Each time version of a project is saved (**commit**), Git creates 'snapshot' of the file and stores a reference to it. Git relies on local operations because most info is found on local resources, which allows for faster processes and ability to work offline. Every change applied to a file/directory is tracked by Git, and file corruption/loss of info is tracked as well. Files in Git take on **committed**, **modified**, and **staged** states. 

**Getting help:** 
- 
```
git help command

git command --help

man git-command
```

## Setting up a git repo

You can import projects/directorys into Git using Terminal/Command Line. 

You can create a copy of an existing Git repo from a server by using clone commands via repo's URL. 

**Cloning:** Create copy of existing Git repo from particular server by using clone command with repo's URL: `git clone <URL>`

## Workflow

### Local repository structure

Local Git repo has three components: **Working directory** (actual files reside here), **Index** (area used for staging), and **Head** (points to the most recent commit). ![Flow](https://blog.udemy.com/wp-content/uploads/2015/08/image036.png)

### Saving changes

All files in progress of being worked on are in a tracked/untracked state. Tracked files can be modified/staged, and untracked files were not in the last snapshot. 

### Life cycle of file status

![Life cycle](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

### Tracking/staging a new file, committing a file, committing all changes, pushing changes, stashing changes

**Tracking/staging a new file:** 
- `git add filename`: tracks one file of your choosing
- `git add *`: tracks all files in repo
- After using these, files are tracked and staged for committing

**Committing a file:**
- `git commit -m "why"`: after staging, changes must be committed, and record what was done
- Committed changes for the file/files to the HEAD
- `git commit -a`: Commits snapshot of all modifications to tracked files in working dir

**Pushing changes:**
- `git push origin master`: pushes changes to remote repo
- Pushed changes from local "master" branch to remote repository called "origin"

**Stashing changes:**
- `git stash`: when changes are not ready to be committed but they do not want to be lost either
- `git stash apply`: when ready to work on changes, retrieves the hidden changes


## Remote repos

In order to collaborate on Git projects, must be able to interact with remote repos (versions of a project online or on a network). It is possible to work with multiple repos (which may have read/write or read-only permissions). Teams may use remote repos to push/pull data to/from. 

## Undoing actions

Git has mechanisms in place to undo actions made to a file (commit mistakes, unstaging a file, undo committed snapshot, unmodifying a file). 

**Commit mistakes:**

- `git commit --ammend`: when you need to alter a commit message or forgot to add files
  - Example: 
  ```
  git commit -m "first commit"
  git add example_file
  git commit --ammend
  ```

**Unstaging a file:**
- `git reset HEAD index.html`: unstages index.html

**Undo committed snapshot:**
- New commit gets appended and rolls back changes from a specific commmit. 
```
git commit -m "message"
git revert HEAD
```


## Branching

Almost every type of VCS incorporates branching. A Git branch is a movable pointer that always points to the *most recent commit (snapshot)*. Git uses the defualt local branch name "master", which can be changed. The head is a special pointer which indicates which branch is being worked within. You can create new branches, switch between branches, create a branch and checkout, and list the branches available. 

![Branching](https://blog.udemy.com/wp-content/uploads/2015/08/image016.png)

## Merging

Branches may be merged from one branch into the current branch. There are various techniques of merging used for what is desired (fast-forward, no fast-forward, three-way, fetch and merge). Branches may be deleted. If two files are being merged and both have changes in *identical* sections of a file, Git will not cleanly merge them, and the conflicts must be dealt with manually. These sections will be labeled as "unmerged". 

## Rebasing

Rebasing is an alternative to merging. There are opposing viewpoints as to which is preferred. The pro-merge argument states that the true commit history of a repo should not be changed because it's a record of what happened. The pro-rebase argument states commit histories should be "polished and well-edited." 

## Logging

Logging commands may be used to view committed snapshots (seeing project's history, find specific modifications, etc). 

## Tagging

Git can flag (Tag) points in a project's history as being something of significance. Tags can be **lightweight** or **annotated**. Users must push tags to shared servers, since the `git push` command does not send tags to remote servers. 

## Aliases

Aliases may be created for Git commands in an effort to expedite Git productivity. 

## Distributed workflows

Every developer on Git can be a node and a hub, which opens up more possibilities for workflows. There are **centralized workflows** and **integration-manager workflows**. 

_this will be edited further once I understand Git and GitHub much more!_
