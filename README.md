# unusual_git_commands

Reference: https://medium.com/mindorks/use-of-git-reset-git-revert-git-checkout-squash-commit-2b721ca2d2d3
### git rebase

### Undo uncommitted changes using git checkout --filename
  git checkout --filename will undo the changes 
  Undo Changes in your Working Directory
  You can use the git checkout command to undo changes you’ve made to a file in your working directory. So, you basically loose all the unstaged changes as the file is reverted     back to the file in HEAD
  
### Undo committed changes using — -> git revert <commitID>
  Rollback changes you have committed.
  Creates a new commit from a specified commit by inverting it. Hence, adds a new commit history to the project, but it doesn’t modify the existing one.
  
  git reset --mixed(default) --hard --soft 
### Delete the most recent commit, keeping the work you've done:
git reset --soft HEAD~1
  
### Delete the most recent commit, destroying the work you've done:
git reset --hard HEAD~1

### Squashing Commits
  git rebase --interactive (used to squash commits and make history look better)
  
  
### The working directory and the staging area/index is shared between branches
  If we make changes in the working directory/staging area of one branch and then we checkout to some other branch without commiting, then those changes would still be visible in the other branch also. But commit history is not shared 
  
