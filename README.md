# Git commands


### Creating a reposiotry online for the first time:-

``` sh
$ git init
# Initialize a repository

$ git add README.md
# add the files you want to the staging area.

$ git commit -m "first commit
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

$ git commit -m “what has changed”

$ git push # ( because I used -u last time)  OR git push origin master

# Enter your username and your password.

```
