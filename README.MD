### <u> Leapfrog Technology Inter Journey </u> ### 
###
### <u> First Assignment of Git </u> ### 
####


### Question 1 : Can we have a global .gitignore? ### 
##
Answer 1 : Yes, we can have a global .gitignore file in Git. .gitignore file is a text file, placed in the root directory that includes specific files which are ignored by Git. It keeps the repository clean, without unnecessary, adapt security measures protecting confidential informations. 
###
In the case of global .gitignore file, it will apply too all Git repositories on my computer. The included files in the global .gitignore file in the root directory ensures us that the information contained in the specified files are not tracked by the Git, no matter the location in my computer. It makes the repository clean by not showing the unnecessary and cluttered information.
##




### Question 2 : How to find difference between two commits? ### 
##
Answer 2 : We can utilize the "git diff" command to find the difference between the two commits. If we have compare commit_1 and commit_2, we can execute the command as:
###
    git diff <sha_commit_1> <sha_commit_2> 
###
Here, sha of each commits can be generated using the command as:
###
    git log --oneline
##



### Question 3 : Write difference between git add and git commit commands.### 

##
Answer 3 : Git add moves the files from the Working Directory to the Staging Area. Git add. It explicitly tells Git which changes we want to include in your next commit as Git doesnot track every change we make in the working directory.
###
Git commit uses records snapshot of your code at a specific point in time as the commits and changes those commit from the Staging Area to the Git Repository. We can go back to the previous versions as all the commited versions are recorded.




##
### Question 4 : How to unstage files? ### 
##
Answer 4 : By using the git reset command, we an unstage files. It moves files from the Staging Area to the Working Directory. To unstage all files that have been added to the staging area as
###
    git reset HEAD


And to unstage a specific file, we specify its name as:
###
    git reset HEAD <file_name>
##



### Question 5 : Difference between revert and reset ### 
##
Answer 5 : The revert command moves the control or current directory to the directory right before the reverted directory and delete the commit specified with is sha from the file itself. It allows to keep a record of the original commit but undo its changes so that the version before the revert command is executed is readily available if needed in the future. The format of revert command is:
###
    git revert <sha_commit>
###
Here, sha of each commits can be generated using the command as:
###
     git log --oneline
###
The reset command is used to permanently erase commits specified with is sha from the commit history. No record of the original commit is found thus, we cannot go back to the version before the reset command was executed even if it is required later. After the reset command, the git commits already in the Git Repository goes back to the Staging Area. The format of reset command is:
###
    git reset <file_name>
##



it