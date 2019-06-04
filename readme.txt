******************Commands********************


C:\Users\sachi\Desktop\sampple_folder>git status

checks for :
1. How many files are modified 
2. Which branch you are
3. How many commits are there
4. How many untracked files are there


Create Empyt file in foleder (with git init) >> text.txt

C:\Users\sachi\Desktop\sampple_folder>git status 
The commnad will show you the above file as "Untracked"


Create Empyt file in foleder (with git init) >> readme.txt

Add some text 

C:\Users\sachi\Desktop\sampple_folder>git status 

You will see "Unmodified" file readme.txt and "Untracked" file test.txt

C:\Users\sachi\Desktop\sampple_folder>git add readme.txt

C:\Users\sachi\Desktop\sampple_folder>git commit

Now readme.txt will not appear in "git status" command


See all previous commits
C:\Users\sachi\Desktop\sampple_folder>git log

C:\Users\sachi\Desktop\sampple_folder>git push Git_Commands master


So, to get updated readme.txt reflected on github :
git add readme.txt
git commit

Add Remote repo to Git
git remote add GitComm https://github.com/JavaShopee/GitCommands.git
git push Git_Commands master


So, to get updated readme.txt reflected on github :
git add readme.txt
git commit
git push Git_Commands master

here Git_Commands is the repository name...


C:\Users\sachi\Desktop\sampple_folder>git remote
Git_Commands  >> that's the repo


C:\Users\sachi\Desktop\sampple_folder>git remote remove Git_Commands

C:\Users\sachi\Desktop\sampple_folder>git remote

C:\Users\sachi\Desktop\sampple_folder>git remote add origin https://github.com/JavaShopee/GitCommands.git

C:\Users\sachi\Desktop\sampple_folder>git remote
origin


Now Edit on github and then git pull

git pull = git fetch + git rebase  

Test Push

