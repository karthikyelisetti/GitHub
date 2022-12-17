**STEP 1: Initialize a new Git project. (Mentioning the command as I have created a subfolder with the project name in the Github Repository)**
	
  > $ git init

<br />

**STEP2: Check the status of the Git project. We will see multiple files listed in the output as “Untracked”.**

  - Create the list of files as in the code academy in the local repo (Working Directory)
  > $ touch disclaimer.txt instructions.txt warranty.txt
   
  - Checking the status of the git project (we notice that there are untracked files that we have added in the above step 2)
  > $ git status

<br />

**STEP 3: Add each file to the Git staging area.**
	
  > $ git add .

<br />

**STEP 4: Check the status of the Git project again. (Now the files are added to the staging area, which are now ready to commit to the local repository (working directory)**
	
  > $ git status

<br />

**STEP 5: Make a commit to the local repository (working directory)**
	
  > $ git commit -m “Adding disclaimer, instructions and warranty files to the main branch”
 
<br />

**STEP 6: Viewing Git commit log. If the cursor is stuck in Git log mode, press “q” on the keyboard to escape.**
	
  > $ git log --oneline --decorate
 
<br />

**STEP 7: Include this line in disclaimer.txt: “Warning: For best battery life, do not leave robot battery charging overnight.”**
	
  > $ vim disclaimer.txt <br />
  > $ cat disclaimer.txt (command used to read the content of the file in the cmd prompt)
 
<br />

**STEP 8: Add the file to the staging area and checking the status of the git project in the local repository (working directory)**
	
  > $ git add disclaimer.txt <br />
  > $ git status
 
<br />

**STEP 9: Now make a commit to the git project in the local repository (working directory)**
	
  > $ git commit -m “Committing the changes to the git project”
 
<br />

**STEP 10: View the Git commit log to identify the commit**
	
  > $ git log --oneline

<br />

**STEP 11: Revise each file in whatever ways we like. Then add the changes to the staging area and make another commit. (The changes will be updated in the local repository (working directory)**

  - Modifying instructions.txt file by adding the text to the Voice commands: “Run” and “Smart thinking!”
  - Modify the warranty.txt file by adding “Note: Any product purchase has a warranty of 1 year” (now we are able to see the files in the green colour as they are modified)
	
    > $ vim instructions.txt <br />
    > $ vim warranty.txt
 
  - Add the file to the git project
  - Commit the files: instructions.txt and warranty.txt  	
	
    > $ git add instructions.txt warranty.txt <br />
    > $ git commit -m “updated the instructions and warranty files”

<br />

**STEP 12: Finally push the changes to the remote repository (This will update the changes in the local repository (working directory) to the remote repository**
	
  > $ git push origin main
 
