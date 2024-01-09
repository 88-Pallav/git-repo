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







