## Introduction
1. if alot of people are working on product, which is ideally the case. For sepearte work, seperate branches are made.
2. use of branch - multiple people can work on the same code and merge it.

## Branch commands
1. `git branch` : to see all the branches that are there and also to see which branch you are on. the branch that you are on is usually highlighted with green color.
2. `git branch -M main` : to rename the branch
3. `git checkout <branch-name>` : to navigate, to move from one branch to another
4. `git checkout -b <new-branch-name>` : to create a new branch
5. `git branch -d <branch-name>` : to delete a branch. you would not be able to delete a branch while you are already in it. you need to switch branches and then delete.
6. once you are in a different branch say branch1, now whatever changes you make will only be reflected in that branch and not in the main one.
7. branches in git are stored as a tree.
8. to have these branch changes seen on github - `git push origin branch1`.
9. you will see a compare and pull request on github once you run the above code.

## Merging code

There are 2 ways of merging branches : 
1. First method - CLI
    1. `git diff <branch-name>` : to compare commits, branches, files and more. it compares your current branch with the one you mention in the command.
    2. `git merge <branch-name>` : to merge 2 branches.
2. Second method - using GitHub
    1. create a pull request - it lets you tell others about the changes you have pushed to a branch in a repo on GitHub.
    2. someone that has access to the main branch reviews the PR first, comments on the request.
    3. to merge - add a new message, make sure to double check the base branch and the branch that you currently are in on github.


Whatever changes you make in main once you create a branch is not reflected in branch.
conflicts can arrise in a pull request if in the main and in the branch, there are changes on the same line of code.
it is up to the person who has access to the main branch to accept that pull request or not.
conflicts are automatically checked by github 

## Pull commands
Once the branches have been merged on GitHub, we need to get those remote changes to our local system. and that can be done using pull command.

1. `git pull origin main` : used to fetch and download content from a remote repo and immediately updated the local repo to match that content.

important to first pull the changes from github and then make new changes to the file.


(this markdown file was written in main)