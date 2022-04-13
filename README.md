# WELCOME TO THE GIT CHEATSHEAT

### 01 GIT CONFIGURATION

 `$ git config --global user.name “Your Name”`

 Set the name that will be attached to your commits and tags.

`$ git config --global user.email “you@example.com”`

 Set the e-mail address that will be attached to your commits and tags.

### 02  STARTING A PROJECT

`$ git init [project name]`

Create a new local repository. If [**project name**] is provided, Git will CREATE a new directory name and will intialise a repository in it.

### 03 DAY TO DAY WORK
`$ git status`

DISPLAY the status of your **working directory**

`$ git add [**file**]`

Add a file to the staging area. Use in place of the full file path to add all changed files from the current directory down into the directory tree.

`$ git commit`

Create a new commit from changes added to the staging area. The commit must have a message!

`$ git rm [file]`

Remove file from **working directory** and staging area.

`$ git stash pop`

Apply stored stash content into **working directory**, and clear stash.

`$ git stash drop`

Delete a specific stash from all your previous stashes. 

### 04 Git branching model
`$ git branch [-a]`

List all local branches in repository. With -a: show all branches [remote]

`$ git branch [branch_name]`

Create new branch, referencing the current HEAD.

`$ git merge [from name]`

Join specified [from name] branch into your current branch.

`$ git branch -d [name]`

Remove selected branch, if it is already merged into any other. 

### Review of your work

`$ git log [-n count]`

List commit history of current branch. -n count limits list to last n commits.

`$ git log --oneline --graph --decorate`

An overview with reference labels and history graph. One commit per line.

`$ git log ref..`

List commits that are present on the current branch and not merged into ref.

`$ git log ..ref`

List commit that are present on ref and not merged into current branch.

`$ git reflog`

List operations (e.g. checkouts or commits) made on local repository.
