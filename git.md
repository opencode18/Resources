

### Table of contents

1. [What is Git?](#whats-a-version-control-system)  
2. [Install Git](#install-git)  
3. [Create A New Repository](#create-a-new-repository)  
4. [Clone A Repository](#clone-a-repository)  
5. [Add & Commit](#add-commit)  
6. [Pushing Changes](#pushing-changes)  
7. [Branching](#branching)  
8. [Update & Merge](#update-merge)     
9. [Replace Local Changes](#replace-local-changes)  

If you are too lazy to read, just skip the two sections :p

### What’s a version control system?
A version control system, or VCS, tracks the history of changes as people and teams collaborate on projects together. As the project evolves, teams can run tests, fix bugs, and contribute new code with the confidence that any version can be recovered at any time. Developers can review project history to find out:

> Which changes were made?
Who made the changes?
When were the changes made?
Why were changes needed?


### What’s a distributed version control system?
Git is an example of a distributed version control system (DVCS) commonly used for open source and commercial software development. DVCSs allow full access to every file, branch, and iteration of a project, and allows every user access to a full and self-contained history of all changes. Unlike once popular centralized version control systems, DVCSs like Git don’t need a constant connection to a central repository. Developers can work anywhere and collaborate asynchronously from any time zone.

Without version control, team members are subject to redundant tasks, slower timelines, and multiple copies of a single project. To eliminate unnecessary work, Git and other VCSs give each contributor a unified and consistent view of a project, surfacing work that’s already in progress. Seeing a transparent history of changes, who made them, and how they contribute to the development of a project helps team members stay aligned while working independently.


Lets Begin
===================

Install Git
-------------

Linux : `sudo apt-get install git`
Windows:  [Download Link](https://github.com/git-for-windows/git/releases/download/v2.15.1.windows.2/Git-2.15.1.2-64-bit.exe)

### Create A New Repository
create a new directory, open it and perform a `git init` to create a new git repository.

### Clone A Repository
create a working copy of a local repository by running the 
command `git clone "url"`

> NOTE :
workflow-
your local repository consists of three "trees" maintained by git. the first one is your `Working Directory` which holds the actual files. the second one is the `Index` which acts as a staging area and finally the `HEAD` which points to the last commit you've made.

###  Add & Commit
You can propose changes (add it to the Index) using `git add <filename>` for particular file and `git add *` for all the changed files
This is the first step in the basic git workflow. To actually commit these changes use `git commit -m "Commit message"` .
Now the file is committed to the HEAD, but not in your remote repository yet.

### Pushing Changes
Your changes are now in the HEAD of your local working copy. To send those changes to your remote repository, execute `git push origin master` .
> Change master to whatever branch you want to push your changes to. 

If you have not cloned an existing repository and want to connect your repository to a remote server, you need to add it with
`git remote add origin <server>`
Now you will be able to push your changes to the selected remote server

### Branching
Branches are used to develop features isolated from each other. The master branch is the "default" branch when you create a repository. Use other branches for development and merge them back to the master branch upon completion.

create a new branch named "feature_x" and switch to it using
>`git checkout -b feature_x`

switch back to master
> `git checkout master`

delete the branch again
> `git branch -d feature_x`

a branch is not available to others unless you push the branch to your remote repository
>-`git push origin <branch>`

### Update & Merge
to update your local repository to the newest commit, execute 
>git pull

in your working directory to fetch and merge remote changes.
to merge another branch into your active branch (e.g. master), use
>git merge "branch"

in both cases git tries to auto-merge changes. Unfortunately, this is not always possible and results in conflicts. You are responsible to merge those conflicts manually by editing the files shown by git. After changing, you need to mark them as merged with
>git add "filename"

before merging changes, you can also preview them by using
>git diff "source_branch" "target_branch"

### Replace local changes
In case you did something wrong, which for sure never happens ;), you can replace local changes using the command
>git checkout -- "filename"

this replaces the changes in your working tree with the last content in HEAD. Changes already added to the index, as well as new files, will be kept.

If you instead want to drop all your local changes and commits, fetch the latest history from the server and point your local master branch at it like this
>git fetch origin
git reset --hard origin/master

