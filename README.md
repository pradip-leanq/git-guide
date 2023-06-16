<!--  Git Flow guide readme file -->

# Git Guide

### Branches

- `main` - main branch
- `dev` - development branch
- `feat/` - feature branch
- `fix/` - bug fix branch
- `hotfix/` - hotfix branch

### Main Branch

Main branch is the main branch of the project. It is the branch that is deployed to production. It is protected and cannot be pushed to directly. It can only be updated by merging a pull request.

### Development Branch

Development branch is the branch that is used for development. It is protected and cannot be pushed to directly. It can only be updated by merging a pull request.

### Feature Branch

Feature branch is the branch that is used for developing a new feature. It is created from the development branch. It is protected and cannot be pushed to directly. It can only be updated by merging a pull request.

### Bug Fix Branch

Bug fix branch is the branch that is used for fixing a bug. It is created from the development branch. It is protected and cannot be pushed to directly. It can only be updated by merging a pull request.

### Hotfix Branch

Hotfix branch is the branch that is used for fixing a bug in production. It is created from the main branch. It is protected and cannot be pushed to directly. It can only be updated by merging a pull request.

### Pull Requests

Pull requests are used to merge a branch into another branch. Pull requests are required to be reviewed and approved by at least one other developer before they can be merged.

<!-- merge workflow -->

### Merge Workflow

1. Create a new branch from the development branch
2. Make changes to the new branch
3. Commit changes to the new branch
4. Push the new branch to the remote repository
5. Create a pull request to merge the new branch into the development branch
6. Review and approve the pull request
7. Merge the pull request
8. Delete the new branch

### Commit Messages

- `feat:` - for new features
- `fix:` - for bug fixes
- `docs:` - for documentation changes
- `style:` - for formatting, missing semi colons, etc; no code change
- `refactor:` - for refactoring production code
- `test:` - for adding tests, refactoring test; no production code change
- `chore:` - for updating build tasks, package manager configs, etc; no production code change

### Git Commands

### Useful Git Commands

- `git init` - initialize git repository
- `git add .` - add all files to staging area
- `git commit -m "message"` - commit changes
- `git branch` - list branches
- `git branch -a` - list all branches
- `git branch branch-name` - create branch
- `git checkout branch-name` - switch to branch

- `git checkout -b dev` - create and switch to dev branch
- `git checkout -b feat/branch-name` - create and switch to feature branch
- `git checkout -b fix/branch-name` - create and switch to bug fix branch
- `git checkout -b hotfix/branch-name` - create and switch to hotfix branch
- `git merge branch-name` - merge branch into current branch
- `git branch -d branch-name` - delete branch
- `git push origin branch-name` - push branch to remote
- `git push origin --delete branch-name` - delete remote branch
- `git push origin :branch-name` - delete remote branch
- `git pull` - pull latest changes
- `git pull origin branch-name` - pull branch from remote
- `git fetch` - fetch latest changes
- `git fetch origin branch-name` - fetch branch from remote
- `git rebase branch-name` - rebase current branch onto branch
- `git rebase --continue` - continue rebase after resolving conflicts
- `git rebase --abort` - abort rebase
- `git stash` - stash changes from working directory
- `git stash pop` - apply stashed changes to working directory
- `git reset HEAD~1` - undo last commit
- `git reset --hard HEAD~1` - undo last commit and remove changes
- `git log` - show commit history
- `git log --oneline` - show commit history (compact)
- `git log --graph --oneline --all` - show commit history (compact graph)
- `git log --stat --summary` - show commit history (detailed)
- `git log --patch` - show commit history (very detailed)

### Git Aliases

- `git config --global alias.co checkout` - git co
- `git config --global alias.br branch` - git br
- `git config --global alias.ci commit` - git ci
- `git config --global alias.st status` - git st
