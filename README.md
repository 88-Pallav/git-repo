# Header

To add a file locally created to git:
git init  // This initialises the empty git repository but to push this live 
             you need to create an empty repository on github

To add this we use remote command:
git remote add orgin "github_https/ssh_link"    // This is done so that we can push changes to origin 
                                                   (It would not recognize origin otherwise)

To check if all is ok run:
git remote -v       // This shows any remote directories connected to this repo
                       (Now we can freely use git pusg origin master/main)


To check the status/track of all the files created adn deleted in a repo: 
git status

So track a file we can do: 
git add "File_name"

Note: First save the file and then proceed for commit

To ensure git keeps track of all the files in a repo:
git add .   // When you use "." then it keeps track of all the files automatically 
               otherwise you have to mention mofdified File name everytime.

To commit something new:
git commit -m "Title Description" -m "Detailed discription"

To upload the changes on github:
git push origin master

To avoid writing the whole thing (git push origin master) we can do:
git push -u origin master       // "-u" is for upstream
                                   (After this can we can use 'git push' only we need not
                                   use mention 'git psuh origin master')


Note: When you create a repo using GUI the above command changes from master to main:
      git push origin main


Summary: 
a. Make the changes
b. Save the changes
c. add the changes (git add .)
d. commit the changes (git commit)
e. push the changed (git push)

To check the branches in repo: 
git branch

To add a branch to a repo:
git checkout -b "branch_name"       // Eg. feature-readme-instructions

To jump to the other branch:
git checkout "branch_name"          // '*' marks the current branch

To compare difference between two branches:
git diff "branch_name"              // You have to be in on the other branch eg. master for this one

To delete a branch:
git branch -d branch_name           // To create: git checkout -b "new branch_name"
                                       To delete: git branch -d branch_name

// To merge just create a pull request and then go on to confirm it on GUI

// After pull request completes type: git pull (To merge the branches)

To add and commit together:
git commit -am "Message"

Merge Conflict 00:47:00 onwards

Undoing add (Undoing staging): 
git reset file_name

Undoing commit:
git reset HEAD~1
// ~1 means going one commit behind and stages last changes 

To see log of all the commits:
git log

// To undo a particular commit copy the hash of the commit:
git reset commit_hash

To remove all the changes:
git reset --hard commit_hash

To remove all the changes:
git reset --hard commit_hash

-------------- Forking ----------------
To completly 'copy' a repo genrally other's repo. It is done to:
a. To create a pull request to be able to contribute changes to the repo
b. To create a branch and do as needed  










