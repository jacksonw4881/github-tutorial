# GitHub Tutorial

_by Jackson Wu_

---
## Git vs. GitHub:

* **Git:** A version control to track your changes.  
  * **Git is not required for github**
  * **Runs in Command Line**
  * **Git is used in a local repositiory** 
   

* **Github:** A website that works using git that holds your code. 
   * **Git is required for github**
   * **Used to collaborate on files with other people**
   * **Github holds and stores changes you've made**

---
## Initial Setup:
    
**_How to create a github account_**: 

1. Go to Github.com [here](http://github.com)
2. Click "sign up" on the top right hand corner 
3. Create a username for the username section (If you're an HSTAT student, put in your HSTAT email without the @hstat.org)
4. Put your email in the email section (Your own personal email or your school's email)
5. Create a password (Something easy to remember, like your ID number)
6. Click on "sign up for GitHub"
7. Click "create an account"
8. Choose the free plan or the paid plan that costs $7
9. Click "continue"
10. Complete the survey and click "submit" (Or skip the survey by clicking "skip this step")  

_Voila! You've just created your GitHub account_ :) 

**Once you've created your GitHub account, you'd need to link an SSH Key from Cloud 9 to GitHub. An SSH key is used to keep your files secure and used to connect the local repository to the remote repository.**

**_How to link an SSH Key from Cloud 9 to GitHub (Assuming you're using Cloud 9 for your IDE):_**

1. Go to your Cloud 9 dashboard
2. Click on the gear icon on the top right corner
3. Click on the SSH Keys on the left hand side
4. Copy your second SSH key (Should start with ssh-rsa and a whole bunch of letters and numbers)
5. Go to your GitHub dashboard on Github.com
6. Click on your profile icon on the top right corner and click on setting
7. Click on "SSH and GPG keys" on the left hand side
8. Click on "New SSH Key"
9. Put a title for the title section
10. Paste in your key in the key section
11. Click "add SSH key"
12. Go to your Cloud 9 terminal and type in "ssh -T git@github.com" and enter. If you've done it successfully, it should say "Hi (your username)! You've successfully authenticated, but GitHub does not provide shell access."

_Voila! You've just linked your SSH key from cloud 9 to GitHub_ :)

---
## Repository Setup:

**Once you've created your GitHub account and linked your SSH Key, you'd need to create a repository on GitHub. GitHub holds remote repositories that can be used to store your files and store changes to those files.**

**_How to create a repository on GitHub:_**

1. Go to Github.com [here](http://github.com) 
2. Click on the plus icon on the top right corner
3. Click on "New Repository"
4. Add a name for your repository (And a description if you'd like)
5. Click "Create repository"
6. If it's on HTTPS, change it to SSH. If it's already on SSH when you've created the repository, leave it.

**After creating your repository, you have to send your changes you've done on your file(s) from Cloud 9 to your remote repository on GitHub.**

**_How to create, add, commit and push your file to GitHub:_**

1. Go to your Cloud 9 terminal
2. Type and enter ```mkdir reponame``` to create a directory and then type and enter ```cd reponame``` to move to that directory (Make sure you're not in any sub directories)
3. Type and enter ```touch README.md``` to create a file within that directory and then type and enter```git init``` to initalize git within that directory
4. Open and edit your file (optional)
5. Type and enter```git add README.md``` to add your file to the staging area
6. Type and enter```git commit -m "commit message"``` to commit that file
7. Go back to Cloud 9 and copy, paste and enter ```git remote add origin git@github.com:username/reponame.git``` from your github repository onto your c9 terminal 
8. Afterwards, copy, paste, and enter ```git push -u origin master``` from your github repository onto your c9 terminal 
 
_Voila! You've just created your first repository and pushed your changes to your remote repository_ :)
