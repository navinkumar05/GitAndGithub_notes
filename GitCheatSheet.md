## Git configuration

```bash
# version check 
git --version git -v 

# Configure Git 
	# Set the name 
	git config --global user.name "navinkumar" 
	# Set the email 
	git config --global user.email "navinkumarpoongkodi@gmail.com" 
	# Set the default editor 
	git config --global core.editor "code --wait" 
	# here i set vscode code editor 
	# Check the setting: 
	git config --list
```
## Starting a project

```bash
# Create a local repository
git init [project name]

# Make a local copy of the server repository
git clone [remote repo URL]
```
## Local changes

```bash
# adding files to staging area
git add .
git add <file name>

# commit
git commit -m "commit message"

git add . && git commit -m "commit message"
```
## Track changes / Inspecting

```bash
# Track the changes that have not been staged:
git diff
# Track the changes that have staged but not committed:
git diff --staged
# Track the changes after committing a file:
git diff HEAD
# Track the changes between two commits:
git diff [commit1-sha] [commit2-sha]
# Git Diff Branches
git diff [branch 1][branch 2]
```
## undoing changes

```bash

git reset --soft
git reset --hard

git revert [commit sha]
git revert --continue
```
## Removing files

```bash 
# Remove the files from the working tree and from the index
git rm
git rm [file name]

# Remove files from the Git But keep the files in your local repository
git rm --cached [file name]
```
## Branch

```bash

# list the branch
git branch

# Switch between branches
git checkout [branch name]
# Create a new branch and switch to it
git checkout -b [branch name]

# Delete Branch
git branch -d [branch name]

# rename branch
git branch -m [old branch] [new branch]

```
### merging
```bash
# rebase
git rebase [branch 1] [branch 2]
git rebase --continue

# merge
git merge [branch 1] [branch 2]

# cherry pic

# stash
```

## git alises

```bash
# use "" if commmand have space
git config --global alias.lo "log --oneline"

git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
```