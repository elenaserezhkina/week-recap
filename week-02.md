# week2-recap

This week we 

## What is Git

Git is ~~GitHub~~ a system for tracking changes in a code. It was created by Linus Torvalds.
_____
### Some commands learned:

1. Create repositories
##### `git init`
Turn an existing directory into a git repository
##### `git clone [url]`
Clone (download) a repository that already exists on
GitHub.

2. Work with branches
#### `git checkout -b branch-name`
create a new branch and switch to it
####  `git branch -d branch-name`
delete the specified branch

3. Pull and push

First of all we pull all the changes from the master by going to the master branch `git checkout master`. Then we execute `git pull` to update our current local working branch with all new commits from the corresponding remote branch on GitHub. 
Then we open code edditor `open .` and make changes to the code.
After all changes are done we check modified files in working directory`git status`.
Next steps are: 
* `git add .`
* `git commit -m "what changes were done"`
* `git push origin branch-name`

! IMPORTANT 
**never push or delete master**

____
### Some essentials:
[Git cheatsheat](https://education.github.com/git-cheat-sheet-education.pdf)


