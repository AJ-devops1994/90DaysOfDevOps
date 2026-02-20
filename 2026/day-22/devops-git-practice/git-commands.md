**git commands for day to day use**

**setup and config**:
- git --version : to check if git is installed along with the version
- sudo apt-get update
- sudo apt install git
- git config --global user.name <user_name>
- git config --global user.email <email id to be used to create your github account>

**Basic workflow**:
- git init : it will initialize the git and will cretae a .git directory in your system
- git remote -v : to check if any remote repository is associated with your local repo
- git remote set-url origin https://<token-generated-from-github-settings>@github.com/<github-user-name>/<remote-repo-name> : to associate local and remote repo
- ssh-keygen : for ssh connection, just store the public key in your github account
- git clone <copy-web-url> : to clone remote repository on your local
- git add <file_name> : stages changes from your working directory to the staging area
- git add . : used to add all the untracked files to staging area in one go
- git commit -m "commit message" : to track the changes in your local git repo
- git rm <file_name> : this will remove the file from your file system but file will still be there in staging area and can be restored anytime.

**Viewing changes**
- git status : to check the status, whether the file is untracked/in staging area/tracked
- git log : to check the detailed logs
- git log --oneline : to check the logs in oneline

**Branching**
- git branch : to check all existing branches along with the pointer to current branch being used
- git checkout -b <branch_name> : to create a new branch and checkout to that branch
- git checkout/switch <branch_name> : to switch to any other existing branch
- git merge <branch_name> : switch to parent branch first. then run this command
- git push origin master : to push the changes to remote repo
- git pull origin master : to pull the changes from remote repo

**Different operations to be performed**
- git pull origin main --rebase : used, in case local and remote branches are not aligned
- git stash : to hide your current working file, to work on other priority task
- git stash pop : to resume your work back
- git cherry-pick <commit_id> : instead of merging all the changes you can cherry-pick a specific commit id to be merged to the parent branch
- git merge <branch_name: to be merged to the current branch> --squash : to squash multiple commits into one and merge with the parent branch
- git revert <commit_id>> : will revert the changes done under particular commit, but it will get reflect in commit history
- git reset --soft 50e0670 : it will remove all the commits after the mentioned commit id(remove commit id and bring back your working tree at current state)

