	Git Command         |       Description
----------------------------|------------------------------------------------------
git init                    | initialize an empty repository
git status                  | Displays paths that have differences between the index file and the <br> current HEAD commit, paths that have differences between the working <br>tree and the index file, and paths in the working tree that are not tracked<br> by Git (and are not ignored by gitignore).
git add filename filename_2 | to add a file so it will be tracked (adds files from the working directory<br> to the staging area)
git diff 		    | shows the difference between the working directory and the staging area<br> (for only the files that are being tracked)
git commit -m "message"     | permanently stores file changes from the staging area in the repository
git log                     | to show commit history

	Git Command         |       Description
----------------------------|------------------------------------------------------
git show HEAD 		    | display everything the git log command displays for the HEAD commit, plus all the file<br> changes that were committed. (The commit we are currently on is called the HEAD commit.<br> In many cases, the most recently made commit is the HEAD commit)
git checkout HEAD filename  | Discards changes in a certain file in the working directory.<br> In other words, the file content will return to what it was when the file was committed.
git reset filename          | Unstages file changes in the staging area.
git reset SHA               | Can be used to reset to a previous commit in your commit history (detaches head)
git clean -i                | remove the files that are not being tracked in the working directory. 
git branch                  | to check what branch we are on.
git checkout branch_name    | to change branch
git merge branch_name       | merge branch_name with the current branch (the current branch is the recieving branch)
git branch -d branch_name   | delete a branch

	Git Command         	     |       Description
-------------------------------------|------------------------------------------------------
git clone remote_location clone_name | clone a remote repository
git remote -v 			     | list the remotes of the project
git remote add origin <server> 	     | add local repo to a remote server
git fetch 			     | fetch the remote changes made by some other people 
git merge origin/master 	     | merge the repo with the master
git push origin your_branch_name     | push your branch up to the remote, origin. 

to revert to a previous commit, use this:
```bash
git reset --hard ##commit# ###
git push --force
```