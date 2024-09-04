### Case 1 : staged changes
1. those changes that have been added but have not been committed.
2. `git reset <file-name>` 
3. `git reset` - for alot of files

### Case 2 : commit some change
1. those changes that have been added and committed, for one commit only 
2. `git rest HEAD~1` - by deafualt the last commit internally in git is stored as HEAD. so this command resets head by one step.
3. can use `git log` to see all commits. to quit the log use - `q`

### Case 3 : commit many changes
1. all commits have an unique hash paired with it.
2. go to `git log` -> find your commit -> copy the hash -> `git reset <hash>` -> `git status` -> `git log`
3. basically these commands help you undo till the add step.
4. say you want to go back to the original unmodified that is undoing the commit and add step, the command for that is - `git reset --hard <hash>`


