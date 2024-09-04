## Resolving merge conflicts
1. an event that takes place when git is unable to automatically resolve differences in code between 2 commits.
2. same line and same file changes.
3. you can check the difference using `git diff main` from that particular branch
4. run `git merge main`, on vscode you have the following options - 
    1. accept current change - accepting branch1/ or whatever branch you are at change.
    2. accept incoming change - main branch changes
    3. accept both changes - both of them will be seen on seperate lines.

(this situation is such that you are in a branch and you merge that with main, so your current branch - branch1 and incoming - main)