# notes_git
This repository store the important command to manage a git repository, I use it personally as a note and it showcase the level of my skills in git.

List of commands:
* [Doawnload a online repository onto your local machine](#download_a_online_repository_onto_your_local_machine)
* [Create a new branch](#create_a_new_branch)
* [Switch to another branch](#switch_to_another_branch)
* [Reset a local branch to its online repository version](#reset_a_local_branch_to_its_online_repository_version)
* [Remove the non-commited/untrack files or directories changes of a local branch](#remove_the_non-commiter_untrack_files_or_directories_changes_of_a_local_branch)
* [Delete a local branch](#delete_a_local_branch)
* [Delete a online branch](#delete_a_local_branch)
* [Upload changes of a local branch onto its online branch](#upload_changes_of_a_local_branch_onto_its_online_branch)
* [Check the change between commits and working tree](#check_the_change_between_commits_and_working_tree)
* [Move a secondary branch to a master branch](#move_a_secondary_branch_to_a_master_branch)
  

<a name="download_a_online_repository_onto_your_local_machine"></a>
#### 1. Download a online repository onto your local machine:
```
git pull <URL>
```
---------------------------------------------------------------
<a name="create_a_new_branch"></a>
#### 2. Create a new branch:
```
git checkout -b <branch_name>
```
---------------------------------------------------------------
<a name="switch_to_another_branch"></a>
#### 3. Switch to another branch:
```
git checkout <branch_name>
```
---------------------------------------------------------------
<a name="reset_a_local_branch_to_its_online_repository_version"></a>
#### 4. Reset a local branch to its online repository version:
```
git checkout <branch_name> -- .
```
---------------------------------------------------------------
<a name="remove_the_non-commiter_untrack_files_or_directories_changes_of_a_local_branch"></a>
#### 5. Remove the non-commited/untrack files or directories changes of a local branch:
```
git clean -n    # shows you the untracked files that would be removed
git clean -f    # removes the untracked files
git clean -dn   # shows you the untracked the directoris that would be removed
git clean -df   # removes the untracked directories
```
---------------------------------------------------------------
<a name="delete_a_local_branch"></a>
#### 6. Delete a local branch:
```
git branch -d <branch_name>
```
---------------------------------------------------------------
<a name="delete_a_online_repository_branch"></a>
#### 7. Delete a online repository branch:
```
git push origin -d <remote_branch_name>   # the remote name is not always origin
```
---------------------------------------------------------------
<a name="upload_changes_of_a_local_branch_onto_its_online_branch"></a>
#### 8. Upload changes of a local branch onto its online branch:

  * Commit of the changes of the local branch:
```
git add .
git status
git commit -m "Message describe the changes"
git status
```
  * Commit the changes of specifics file and repository of the local branch:
```
git add <file_or_repository_1> <file_or_repository_2>
git status
git commit -m "Messahe describe the changes"
git status
```  
  * Push/Upload the commit change of the branch online:
```
git push origin <branch_name>
git status
```
---------------------------------------------------------------
<a name="check_the_change_between_commits_and_working_tree"></a>
#### 10. Check the change between commits and working tree:
```
git diff <commit> <commit>
```
---------------------------------------------------------------
<a name="move_a_secondary_branch_to_a_master_branch"></a>
#### 11. Move a secondary branch to a master branch:
```
git push -u origin <new_default-branch>
```
