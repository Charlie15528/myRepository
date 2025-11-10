# Git Application Answers

## Question 1: Reverting Modifications

### Method 1: Using `git restore`
```bash
# Discard changes in working directory for specific file
git restore <filename>

# Discard all changes in working directory
git restore .
new lines edited
# Git Application Answers

## Question 1: Reverting Modifications

### Method 1: Using `git restore`
```bash
# Discard changes in working directory for specific file
git restore <filename>

# Discard all changes in working directory
git restore .
# Unstage files but keep changes in working directory
git reset

# Discard all changes in working directory
git checkout -- .
# Completely reset to last commit (loses all changes)
git reset --hard HEAD
# Create a new commit that undoes the changes
git revert <commit-hash>
# Restore files to previous commit state
git restore --source=HEAD~1 <filename>
# Move HEAD back but keep changes staged
git reset --soft HEAD~1
# Completely remove the last commit and all changes
git reset --hard HEAD~1
# Standard merge creating a merge commit
git checkout main
git merge feature-branch
# Rebase feature branch onto main
git checkout feature-branch
git rebase main

# Fast-forward merge
git checkout main
git merge feature-branch
# Squash all commits from feature branch into one
git checkout main
git merge --squash feature-branch
git commit -m "Squashed feature branch"
