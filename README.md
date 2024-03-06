# Header

How to bring a repository on Github to a local Machine?
Step 1: Create an empty repository on Github.
Step 2: In VS Code got to terminal
Step 3: Open a folder where you want the repository to be cloned.
Step 4: Then in terminal use the command: git clone SSH_key_of_the_repository
Step 5: Get into the folder by using: cd folder_name_created_on_github
Step 6: Start using the same.     


*To check the status/track of all the files created and deleted in a repo:* 
git status

*So track a file we can do, track is for files created on local machine but not on github:* 
git add "File_name"

Note: First save the file and then proceed for commit

*To ensure git keeps track of all the files in a repo:*
git add .   // When you use "." then it keeps track of all the files automatically 
               otherwise you have to mention mofdified File name everytime.

*To commit something new:*
git commit -m "Title Description" -m "Detailed discription"

*To upload the changes on github:*
git push origin master

*To avoid writing the whole thing (git push origin master) we can do:*
git push -u origin master       // "-u" is for upstream
                                   (After this can we can use 'git push' only we need not use mention 'git push origin master')
                
Note: When you create a repo using GUI the above command changes from master to main:
      git push origin main


How to create a file on local machine and connect it to Github ? 
Step 1: Create a file in a folder in your local machine.
Step 2: Move into that folder using cd
Step 3: Create a file in that fodler
Step 4: Then use the command: git init  // To initialize the git repository in the folder
Step 5: Then check with command: git status 
Step 6: Add the same the using command: git add
Step 7: To push it live: first create an empty repository on GitHub
Step 8: To connect use command: git remote add origin ssh-key
Step 9: To check the connection: git remote -v
Step 10: To push the changes we need to do: git push -u origin master


*To add a file locally created to git:*
git init          // This initialises the empty git repository but to push this live 
                     you need to create an empty repository on github

*To add this we use remote command:*
git remote add origin "github_https/ssh_link"    
// This is done so that we can push changes to origin (It would not recognize origin otherwise)

*To check if all is ok run:*
git remote -v       // This shows any remote directories connected to this repo
                       (Now we can freely use git push origin master/main)


Summary: 
a. Make the changes
b. Save the changes
c. add the changes (git add .)
d. commit the changes (git commit)
e. push the changed (git push)


******************* Branching **************************

*To check the branches in repo:* 
git branch

*To add a branch to a repo:*
git checkout -b "branch_name"    // Eg. git checkout - b feature-readme-instructions

*To jump to the other branch:*
git checkout "branch_name"       // '*' marks the current branch

*To compare difference between two branches:*
git diff "branch_name"     // You have to be in on the other branch eg. master for this one

*To delete a branch:*
git branch -d branch_name     // To create: git checkout -b "new branch_name"
                                 To delete: git branch -d branch_name

*To merge just create a pull request and then go on to confirm it on GUI. After pull request completes type:* 
git pull (To merge the branches)

*To add and commit together:*
git commit -am "Message"    // Only applicable to modified files and not to new files 

*Undoing add (Undoing staging):* 
git reset file_name

*Undoing commit:*
git reset HEAD~1  // ~1 means going one commit behind and stages last changes 

*To see log of all the commits:*
git log

*To undo a particular commit copy the hash of the commit:*
git reset commit_hash

*To remove all the changes:*
git reset --hard commit_hash

-------------- Forking ----------------
To completly 'copy' a repo generally other's repo. It is done to:
a. To create a pull request to be able to contribute changes to the repo
b. To create a branch and do as needed          


