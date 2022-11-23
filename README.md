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
git remote set-url origin <remote-url>

# TO COMMIT CHANGES
# add files so that you can push to repo
git add .
# commit/confirm your changes
git commit -m "explain what you did, but keep it short and concise"
# <optional> push your changes to Github
git push

#### NICE TO KNOW COMMANDS ####
# See the status of the project files since last commit
git status

# Pull and merge project files from Github Repo
git pull

# Pull project files from Github Repo without merging
git fetch origin
# go into fetched branch
git checkout origin/<branch-name>
### OR ###
# fetch only one branch from repo without merging
git fetch origin <branch-name>
git checkout <branch-name>
# go back to main to "undo" a fetch
git checkout main

# Create and switch to new branch
git checkout -b <branch-name>

# To switch between different branches
git checkout <branch-name>

# To store local changes without committing
git stash 
# To restore local changes
git stash pop

# Reset changes since last commit
git reset --hard HEAD
# Undo last commit
git reset --hard HEAD^ -or- git reset --hard HEAD~1
# Undo second to last commit
git reset --hard HEAD~2
# Undo N^th commit
git reset --hard HEAD~<N>

# See all changes since last commit
git diff
# See changes to file since last commit
git diff <file-name>
```

###### More commands [here](https://github.com/Amark18/Git-Cheat-Sheet/blob/main/Git_Sheet.pdf).
