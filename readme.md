## to discard changes after the last commit 
git reset --hard
(sets pointer to the head)

## to delete last n commits from the log
git reset --hard n

## to delete commit till a specified commit 
git reset --hard <commit-hash>

## to create a new repository with local changes saved that are not commited in the current repository 
### 1. create a new branch
`git checkout -b new-branch`

### 2. add the local changes
`git add .`

### 3. commit the changes to the new branch
`git commit -m "added local changes to the new branch"`

### 4. switch to original branch
`git checkout old-branch`

### 5. clean the local changes so that only commit changes remain
`git clean -f`

