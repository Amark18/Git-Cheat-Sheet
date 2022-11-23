## Git Cheat Sheet
###### Simple and short git cheat sheet for the average programmer.

```shell
# CLONING AN EXISTING REPO 
# note: make sure you are in your desired directory
git clone <remote_url>
# go inside project directory
cd <repo-name>
# <optional> set the remote url so when you push/pull, it goes to GitHub
git remote set-url origin <remote_url>

# TO PUSH TO GITHUB REPO
# add files so that you can push to repo
git add .
# commit/confirm your changes
git commit -m "explain what you did, but keep it short and concise"
# push your changes to Github
git push

#### NICE TO KNOW COMMANDS ####
# see the status of the project files aka changed files
git status

# to get the most updated project files
git pull

# create and switch to new branch
git checkout -b <branch-name>

# To switch between different branches
git checkout <branch-name>

# To store local changes without committing
git stash 
# To restore local changes
git stash pop

# reset changes since last commit
git reset --hard HEAD
# undo last commit
git reset --hard HEAD^ -or- git reset --hard HEAD~1
# undo second to last commit
git reset --hard HEAD~2
# undo N^th commit
git reset --hard HEAD~<N>

# see all changes since last commit
git diff
# see changes to file since last commit
git diff <file-name>

# fetch current state of repo without merging
# essentially just "peeking" at the current state of repo
git fetch origin
# go into fetched branch
git checkout origin/<branch-name>
### OR ###
# fetch only one branch from repo without merging
git fetch origin <branch_name>
git checkout <branch_name>
# go back to main to "undo" a fetch
git checkout main
```
