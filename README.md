## Git Cheat Sheet
###### Simple and short git cheat sheet for the average programmer.

```shell
# CREATE NEW GIT REPO
# note: make sure you are in your desired directory 
git init

# CLONING AN EXISTING REPO 
# note: make sure you are in your desired directory
git clone <remote_url>
# go inside project directory
cd <repo-name>
# <optional> set the remote url so when you push/pull, it goes to GitHub
git remote add origin <remote-url>

# TO COMMIT CHANGES
# add files so that you can push to repo
git add .
# commit/confirm your changes
git commit -m "explain what you did, but keep it short and concise"
# <optional> push your changes to Github
git push

#### NICE TO KNOW COMMANDS ####
# see the status of the project files since last commit
git status

# pull and merge project files from Github Repo
git pull

# pull project files from Github Repo without merging
git fetch origin
# go into fetched branch
git checkout origin/<branch-name>
### OR ###
# fetch only one branch from repo without merging
git fetch origin <branch-name>
git checkout <branch-name>
# go back to main to "undo" a fetch
git checkout main

# create and switch to new branch
git checkout -b <branch-name>

# to switch between branches
git checkout <branch-name>

# to delete a branch locally
git branch -d origin <branch-name>
# to delete remote branch
git push -d origin <branch-name>

# to store local changes without committing
git stash 
# to restore local changes
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
```

###### More commands [here](https://github.com/Amark18/Git-Cheat-Sheet/blob/main/Git_Sheet.pdf).
