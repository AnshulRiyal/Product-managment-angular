# <p align="center">Things Every Developer Must Know:</p>
## Github useful commands

### Clone/Download a repo: 
`git clone <repo-https-url>`

### Clone single branch only:
`git clone <repo-url> --branch <branch-name> --single-branch`

### See local changes: 
`git status`

### Add changed files: 
`git add <filename1> <filename2> <filename3>`

### Add all changed files: 
`git add .`

### Commit changes: 
`git commit -m “<explain your commit>”`

### Push local changes: 
`git push origin <branch_name>`

### Pull server changes: 
`git pull origin <branch_name>`

### Get new branches and codes:
`git fetch`

### Create new branch:
`git branch <branch_name>`


### Create new branch with current changes:
`git checkout -b <branch_name>`

### Switch between branches: 
`git checkout <new_branch_name>`

### Switch to any commit:
`git reset --hard <commit-number>`

### Remove untracked files:
`git clean -f -d`

### Reset .gitignore file changes:
`git rm -r --cached .
git add .
git commit -m ".gitignore updated"`

### Remove all local branches that are not on remote
`git branch --merged master | grep -v '^[ *]*master$' | xargs git branch -d`

### Commit deleted files only
`git add -u`

### Revert Local Commit:
`git reset HEAD~1`

### Git global setup
`git config --global user.name "anshulriyal00@gmail.com"` 
`git config --global user.email "anshulriyal00@gmail.com"`

### To check remote:
`Git remote -v`
OUTPUT:

`origin	https://github.com/AnshulRiyal/developer_baby.git (fetch)`
`origin	https://github.com/AnshulRiyal/developer_baby.git (push)`

### To remane remote origin URL:
`git remote set-url origin https://github.com/AnshulRiyal/developer_babySteps.git`
OUTPUT:

`origin	https://github.com/AnshulRiyal/developer_babySteps.git (fetch)`
`origin	https://github.com/AnshulRiyal/developer_babySteps.git (push)`

### To remove git remote:
`git remote remove <name>` => Where `name` is `origin` in above output. 

### Remove Git tracking from a project:
Open a terminal and navigate to the directory of your project, i.e. - cd path_to_your_project.
Run this command:
`rm -rf .git*`
