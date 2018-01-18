
### Welcome
Hey!  
Beginner? Do not worry you have came to the correct place.  
Here we will give you a brief idea on how to kick start opensource development with github and git.


### Table of contents
1. [What is Github?](#what-is-github?)
2. [Lets Begin](#lets-begin)  
		1.  [Step 1. Create a Repository](#step-1-create-a-repository)  
		2.  [Step 2. Create a Branch](#step-2-create-a-branch)  
		3.  [Step 3. Make and commit changes](#step-3-make-and-commit-changes)  
		4.  [Step 4. Open a Pull Request](#step-4-open-a-pull-request)  
		5.  [Step 5. Merge your Pull Request](#step-5-merge-your-pull-request)  
3. [Forking Projects](#forking-projects)  
4. [What is Git?](#whats-a-version-control-system)  
5. [Install Git](#install-git)  
6. [Create A New Repository](#create-a-new-repository)  
7. [Clone A Repository](#clone-a-repository)  
8. [Add & Commit](#add-commit)  
9. [Pushing Changes](#pushing-changes)  
10. [Branching](#branching)  
11. [Update & Merge](#update-merge)     
12. [Replace Local Changes](#replace-local-changes)  

## Go Resources

### Learn
#### Learn Go Online
* [The Little Go Book](http://openmymind.net/The-Little-Go-Book/)
  * [Exercism.io - Go](http://exercism.io/languages/go) - Online code exercises for Go for practice and mentorship.
  * [Learn Go in an Hour - Video](https://www.youtube.com/watch?v=CF9S4QZuV30) _2015-02-15_
  * [Learning to Program in Go](https://www.youtube.com/playlist?list=PLei96ZX_m9sVSEXWwZi8uwd2vqCpEm4m6), a multi-part video training class.
  * [Pluralsight Classes for Go](http://www.pluralsight.com/tag/golang) - A growing collection of (paid) online classes.
  * [Ardan Labs Training](https://www.ardanlabs.com/) - Commercial, live instruction for Go programming.
  * [O'Reilly Go Fundamentals](http://shop.oreilly.com/category/learning-path/go-fundamentals.do) - Video learning path for Go programming.
  * [Go By Example](http://gobyexample.com/) provides a series of annotated code snippets.
  * [Learn Go in Y minutes](http://learnxinyminutes.com/docs/go/) is a top-to-bottom walk-through of the language.
  * [Workshop-Go](https://github.com/sendwithus/workshop-go) - Startup Slam Go Workshop - examples and slides.
  * [Go Fragments](http://www.gofragments.net/) - A collection of annotated Go code examples.
  * [50 Shades of Go: Traps, Gotchas, Common Mistakes for New Golang Devs](http://devs.cloudimmunity.com/gotchas-and-common-mistakes-in-go-golang/index.html)
  * [Free Go Language Workshop](https://www.frameworktraining.co.uk/go-language-free-training-workshop/) Framework Training is running regular free BYOD workshops in London, UK
  * [GoingGo.net](http://www.goinggo.net/) - A collection of videos and articles for learning Go.
  * [Golang Tutorials](http://golangtutorials.blogspot.com/2011/05/table-of-contents.html) - A free online class.
  * Rob Pike's 2011 three day course - [Day 1](http://go.googlecode.com/hg-history/release-branch.r60/doc/GoCourseDay1.pdf), [Day 2](http://go.googlecode.com/hg-history/release-branch.r60/doc/GoCourseDay2.pdf), [Day 3](http://go.googlecode.com/hg-history/release-branch.r60/doc/GoCourseDay3.pdf) (*links are broken*, use the archived links from the wayback machine. [Day 1][wbday1], [Day 2][wbday2], [Day 3][wbday3])
  * [The Go Bridge Foundry](https://github.com/gobridge) - A member of the [Bridge Foundry](http://bridgefoundry.org/) family, offering a complete set of free Go training materials with the goal of bringing Go to under-served communities.
* [Golangbot](https://golangbot.com/learn-golang-series/) - Tutorials to get started with programming in Go.
* [Master Go](https://appliedgo.com/p/mastergo/) - A paid online video course on Go for developers
* [Learn to Create Web Applications using Go](https://www.usegolang.com/) - A paid online video course and book about Web programming with Go
* [Learn Go Programming](https://blog.learngoprogramming.com) - Weekly visual and concise tutorials for programming in Go.
* [Gophercises](https://gophercises.com/) - coding exercises for budding gophers
* [Crowdsourced List Of Golang Tutorials](https://onlinecourses.guru/submit/edit/topic/learn-go) - Golang tutorials crowd sourced by programmers.


[wbday1]: http://web.archive.org/web/20160305024536/http://go.googlecode.com/hg-history/release-branch.r60/doc/GoCourseDay1.pdf
[wbday2]: http://web.archive.org/web/20160305081012/http://go.googlecode.com/hg-history/release-branch.r60/doc/GoCourseDay2.pdf
[wbday3]: http://web.archive.org/web/20160305075151/http://go.googlecode.com/hg-history/release-branch.r60/doc/GoCourseDay3.pdf

Learning resources for specific topics:
  * [LearnConcurrency](LearnConcurrency) outlines a course of study of Go's concurrency model and patterns.
  * [LearnErrorHandling](LearnErrorHandling) links to resources about error handling in Go.
  * [LearnTesting](LearnTesting) links to resources about testing in Go.
  * [LearnServerProgramming](LearnServerProgramming) links to resources about server programming in Go.
  * [Hackr.io Golang Tutorials](https://hackr.io/tutorials/learn-golang) - Best Golang tutorials recommended by the programming community.

Further reading:
  * [Newspaper](http://www.newspaper.io) is a topic based newsfeed for slack. Built on Go

What is GitHub?
===================
GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

This tutorial teaches you GitHub essentials like repositories, branches, commits, and Pull Requests. You’ll create your own Hello World repository and learn GitHub’s Pull Request workflow, a popular way to create and review code.

----------

Lets Begin
===================

Step 1. Create a Repository
-------------

A repository is usually used to organize a single project. Repositories can contain folders and files, images, videos, spreadsheets, and data sets – anything your project needs. We recommend including a README, or a file with information about your project. GitHub makes it easy to add one at the same time you create your new repository. It also offers other common options such as a license file.

### To create a new repository :
> - In the upper right corner, next to your avatar, click  and then select New repository.
> - Name your repository say "hello-world".
> - Write a short description.
> - Select Initialize this repository with a README.
> - Click Create repository.

![](https://guides.github.com/activities/hello-world/create-new-repo.png)


Step 2. Create a Branch
-------------

Branching is the way to work on different versions of a repository at one time.

By default your repository has one branch named `master` which is considered to be the definitive branch. We use branches to experiment and make edits before committing them to master.

When you create a branch off the master branch, you’re making a copy, or snapshot, of master as it was at that point in time. If someone else made changes to the master branch while you were working on your branch, you could pull in those updates.

This diagram shows:

> - The master branch
> - A new branch called feature (because we’re doing ‘feature work’ on this branch)
> - The journey that feature takes before it’s merged into master

![](https://guides.github.com/activities/hello-world/branching.png)

### To create a new branch :
> - Go to your new repository hello-world.
> - Click the drop down at the top of the file list that says branch: master.
> - Type a branch name, readme-edits, into the new branch text box.
> - Select the blue Create branch box or hit “Enter” on your keyboard.

Now you have two branches, master and readme-edits. They look exactly the same, but not for long! Next we’ll add our changes to the new branch.

![](https://guides.github.com/activities/hello-world/readme-edits.gif)


Step 3. Make and commit changes
-------------

Now, you’re on the code view for your readme-edits branch, which is a copy of master. Let’s make some edits.

On GitHub, saved changes are called commits. Each commit has an associated commit message, which is a description explaining why a particular change was made. Commit messages capture the history of your changes, so other contributors can understand what you’ve done and why.

### Make and commit changes :
> - Click the README.md file.
> - Click the  pencil icon in the upper right corner of the file view to edit.
> - In the editor, write a bit about yourself.
> - Write a commit message that describes your changes.
> - Click Commit changes button.

These changes will be made to just the README file on your readme-edits branch, so now this branch contains content that’s different from master.

![](https://guides.github.com/activities/hello-world/commit.png)

Step 4. Open a Pull Request
-------------

Nice edits! Now that you have changes in a branch off of master, you can open a pull request.

Pull Requests are the heart of collaboration on GitHub. When you open a pull request, you’re proposing your changes and requesting that someone review and pull in your contribution and merge them into their branch. Pull requests show diffs, or differences, of the content from both branches. The changes, additions, and subtractions are shown in green and red.

As soon as you make a commit, you can open a pull request and start a discussion, even before the code is finished.

You can even open pull requests in your own repository and merge them yourself. It’s a great way to learn the GitHub Flow before working on larger projects.


### Open a Pull Request for changes to the README :

> - Click the  Pull Request tab, then from the Pull Request page, click the green New pull request button.

![](https://guides.github.com/activities/hello-world/pr-tab.gif)

> - In the Example Comparisons box, select the branch you made, readme-edits, to compare with master (the original).

![](https://guides.github.com/activities/hello-world/pick-branch.png)

> - Look over your changes in the diffs on the Compare page, make sure they’re what you want to submit.

![](https://guides.github.com/activities/hello-world/diff.png)

> - When you’re satisfied that these are the changes you want to submit, click the big green Create Pull Request button.

![](https://guides.github.com/activities/hello-world/create-pr.png)

> - Give your pull request a title and write a brief description of your changes.

![](https://guides.github.com/activities/hello-world/pr-form.png)

> - When you’re done with your message, click Create pull request!


Step 5. Merge your Pull Request
-------------


In this final step, it’s time to bring your changes together – merging your readme-edits branch into the master branch.

If you are contributing to projects owned by others , then this step will be done by them after reviewing your PR(pull request).

> - Click the green Merge pull request button to merge the changes into master.
> - Click Confirm merge.
> - Go ahead and delete the branch, since its changes have been incorporated, with the Delete branch button in the purple box.

![](https://guides.github.com/activities/hello-world/delete-button.png)

![](./images/flow.PNG)


Forking Projects
===================


After using GitHub by yourself for a while, you may find yourself wanting to contribute to someone else’s project. Or maybe you’d like to use someone’s project as the starting point for your own. This process is known as forking.

Creating a “fork” is producing a personal copy of someone else’s project. Forks act as a sort of bridge between the original repository and your personal copy. You can submit Pull Requests to help make other people’s projects better by offering your changes up to the original project. Forking is at the core of social coding at GitHub.



Fork the repository
-------------

To fork the repository, click the Fork button in the header of the repository.
![](https://github-images.s3.amazonaws.com/help/bootcamp/Bootcamp-Fork.png)

Sit back and watch the forking magic. When it’s finished, you’ll be taken to your copy of the repository.

After Forking make the required changes and commit the changes.

Making Pull Request
-------------
At last, you’re ready to propose changes into the main project! This is the final step in producing a fork of someone else’s project, and arguably the most important. If you’ve made a change that you feel would benefit the community as a whole, you should definitely consider contributing back.

To do so, head on over to the repository on GitHub.com where your project lives. For this example, it would be at `https://www.github.com/your_username/RepoName` . You’ll see a banner indicating that you’ve recently pushed a new branch, and that you can submit this branch “upstream,” to the original repository:

![](https://github-images.s3.amazonaws.com/help/pull_requests/recently_pushed_branch.png)

Clicking on Compare and Pull Request sends you to a discussion page, where you can enter a title and optional description. It’s important to provide as much useful information and a rationale for why you’re making this Pull Request in the first place. The project owner needs to be able to determine whether your change is as useful to everyone as you think it is.

When you’re ready typing out your heartfelt argument, click on Send pull request. You’re done!

![](https://github-images.s3.amazonaws.com/help/pull_requests/pullrequest-send.png)

-----------------------------------------------------------------


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
workflow :  
your local repository consists of three "trees" maintained by git. the first one is your `Working Directory` which holds the actual files. the second one is the `Index` which acts as a staging area and finally the `HEAD` which points to the last commit you've made.

###  Add & Commit
You can propose changes (add it to the Index) using `git add <filename>` for particular file and `git add *` for all the changed files.  
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



### Need any help?
[@mubaris](https://www.facebook.com/nk.mubaris) , [@aswinzz](https://www.facebook.com/aswinvb) , [@aswanthkoleri](https://www.facebook.com/aswanth9495) , [@Anupam-Dagar](https://www.facebook.com/invincible.anupam)
