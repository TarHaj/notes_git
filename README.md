# notes_git
This repository store the important command to manage a git repository, I use it personally as a note and it showcase the level of my skills in git.

1. Download a online repository onto your local machine:
```
git pull <URL>
```
2. Create a new branch:
```
git checkout -b <branch_name>
```
3. Switch to another branch:
```
git checkout <branch_name>
```
4. Reset a local branch to its online repository version:
```
git checkout <branch_name> -- .
```
5. Remove the non-commited/untrack files or directories changes of a local branch:
```
git clean -n    # shows you the untracked files that would be removed
git clean -f    # removes the untracked files
git clean -dn   # shows you the untracked the directoris that would be removed
git clean -df   # removes the untracked directories
```
5. Delete a local branch:
```
git branch -d <branch_name>
```
6. Delete a online repository branch:
```
```
7. Upload change of a branch:

  a. Commit of the changes of the local branch:
```
git add .
git status
git commit -m "Message describe the changes"
git status
```
  abis. Commit the changes of specifics file and repository of the local branch:
```
git add <file_or_repository_1> <file_or_repository_2>
git status
git commit -m "Messahe describe the changes"
git status
```  
  b. Push/Upload the commit change of the branch online:
```
git push origin <branch_name>
git status
```
9. Check the change between commits and working tree:
```
git diff <commit> <commit>
```
10. Change the a secondary branch to a master branch:
```
git push -u origin <new_default-branch>
```
