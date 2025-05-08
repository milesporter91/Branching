## Git Branching Practice

Git cheat sheet and branching practice.

### Basic Commands
* `git init` - initialize local git repo in current folder( working directory)
* `git add` - stage all changes for commit
* `git commit -m "message"` - commit staged changes to local repo

### Info Commands
* `git status` - show current status of working directory
* `git log` - show local commit history
* `git log --oneline` - show local commit history, compact format
*  `git config -l` - list configuration of local repo
* `git config --global -l` - list global configuration
* `git version` - show local git version

### Branching Commands
* `git branch` - list local branches
* `git branch branchName` - create new branch 'branchName'
* `git checkout branchName` - switch to branch 'branchName'
* `git checkout -b branchName` - create and checkout `branchName`

### Remote Commands
* `git remote add alias URL` - connect local repo to remote, useing name `alias` for remote repo `URL`
* `git push alias branchName` - push local commits to remote repo `alias` on branch `branchName`

### Git Branch Workflow
1. Go to local `main` branch
    ```
    git checkout main
    ```
2. Pull remote main
    ```
    git pull origin main
    ``` 
3. Create and check out new branch
    ```
    git checkout -b "branchName"
    ```
4. Work on your branch, committing frequently

5. When task complete, pull main and fix merge conflicts
    ```
    git add .
    git commit -m "message"
    git pull origin main
    ```
6. Push to your branch
    ``` 
    git push origin branchName
    ```
7. Create pull request on GitHub
8. Merge pull request to main
    
