```bash
#GitApplying Problem Solving answers
# Question 1: Roll back changes that have been modified but not committed
## Option 1: Using git checkout
git checkout -- <file>
## Option 2:Using git restore
git restore <file>
## Option 3:Using git reset
git reset --hard HEAD
Problem 2:Revert to a committed version
##Option 1:Using git revert
git revert HEAD
#Option 2:create a reverse commit
git revert <commit-hash>
#The forementioned changes the history
#The following changes no history
#Option 1 :Using git reset --hard
git reset --hard HEAD~1
#Option 2: Using git reset --soft
git reset --softg HEAD~1
##Problem 3:Different ways to merge branches
#Option 1: Using merge
git merge <branch-name>
#Option 2: Using rebase
git rebase <branch-name>
#Option 3:Using chherry-pick
git cherry-pick <commit-hash>
EOF
