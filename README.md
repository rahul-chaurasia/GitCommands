# Git commands


### Creating a reposiotry online for the first time:-

``` sh
$ git init
# Initialize a repository

$ git add README.md
# add the files you want to the staging area.

$ git commit -m "first commit"
# Commit the changes you made.

$ git remote add origin https://github.com/ramanbanka/GitCommands.git
# Connect the staging area to the remote

$ git status
# Check the status of your repository

$ git push -u origin master
# Push(upload) the files in the staging area to the remote.

# Enter your github username and your password.

```

### When adding on to your repository online with changes:

``` sh
$ git add .

$ git add -u 
# When you have deleted a local file you want to remove from your repo

$ git commit -m “what has changed”

$ git push # ( because I used -u last time)  OR git push origin master

# Enter your username and your password.

```

### No more username and input for every push

``` sh

$ git remote set-url origin git$github.com
:yourUsername/yourRepoName.git
#We can find the ssh clone url in the right pane of our repository

```

###  Working together from the perspective of the person that doesn't have the main repo

``` sh

# Fork the repo you want to work on

$git clone https://github.com/yourUsername/yourReponame.git

# change it and push it

# if you want to change the original one, then generate a pull request.

``` 


### Modify offline copy when online copy is already modified

``` sh
$ git pull
```

### Want to remove a file from online github repo but keep it locally

``` sh
$ git rm --cached localfilename

# add localfilename to .gitignore file & then commit these changes

```

### Commands for fixing problems

``` sh

# undo multiple commits

$ git reset --hard commitSHA###...= changes staging index and local folder to match online repository commit.

#removing 3 commits from online github repo

$ git push -f origin HEAD^^^: branchNameToUndoLast3Pushes

```

### Branch Commands


##### Creating a  new branch

```

$ git branch # list all branches in working folder

$ git branch newBranchName

$ git checkout newBranchName # Switch to branch newBranchName

$ git push origin newBranchName # adds new branch to github repo

```

##### Merging new branch to old branch

```

$ git checkout oldBranchName

$ git merge newBranchName

$ git push origin oldBRanchName

```

##### Deleting a branch

```

$ git branch -d branchNameTodelete # Delete branch while you are at a different branch

```
