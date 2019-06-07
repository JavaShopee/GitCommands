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




***********************Git Commands Continued********************************

Unstage from Staging to working file
git reset HEAD first.txt


Move changes from repo to working file
git checkout (commit number) -- filename.txt

When the changes are made to file, not staged or commited
Then we can extract last good copy from Repo 


git checkout -- filename.txt



***********************************************************************************************
Git is a distributed version-control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows.

Change Config Setting
git config --global user.name "Sachin Arora"
git config --global user.email "sacharora99@gmail.com"
git config --list
clear

Check Settings
git config user.email 
git help
git help commit  >> Open commit help page in default browser

Start a git project 
git init
To show all the hidden stuff in folder(.git in our case) , use command:
ls -la
Create a text file readme.txt in above folder generated.Add some text..save..
git add .  >> Add all changes we made to our project.

git commit -m "First Commit"
git log  >> commit history
git log --author="Sachin" >> Just first name will work
git status 

working copy --------------------------->> Staging Area---------------------------------------->>Repository
file created --------------------------->> git add filename.txt--------------------------------->> git commit

files in red shows "Files not yet added"
files in green shows "Files not yet commited"

Viewing the Changes That You Made
git status >> will show you modified files
git diff >> Working copy Vs Repository
git diff --staged >> Staging Vs Repository

Red the previous one and Green, the current one

Now "git add ." and "git commit -m "the message"" and then
git diff will give you no differences from previous file 

Delete Files :
git rm filename.txt  (Do remember to commit after delete, to take the snapshot of this point of time)


Renaming the file :
1. First rename the file manually
2. git add index.txt 
3. git rm first.txt
This will show you file is actually renamed
4. git commit -m "file renamed"

Now from CLI :
Moving the file is same as renaming the file
git mv secondfile.txt newfile.txt

git mv secondfile.txt newfoleder/renamedfile.txt

Commit the eclipse project
browse to the folder >> git add . >> git commit -m "commit the project"

Shortcut :
git commit -am "Commit working copy to repo without adding"
-> Useful when you want to commit entire project(not just one or two file)
-> Do not use while renaming / deleting the files
-> Useful for simple edits only
 
Copy repository file to working file(before commiting):
git checkout -- schema.sql

Unstage the file(from staging to working file):
git reset HEAD schema.sql
In other words, we can stage two times

Go back to previous commits:

git checkout 2c257c9e437e48cd65bf54ca2706ad64f9957b8c -- readme.txt
git checkout (first few initials of commit number) -- readme.txt


git remote add logindemo https://github.com/JavaShopee/DemoRepo.git
git remote
Pushing  Fetch
git push -u logindemo master


Git Ignore
touch .gitignore  >> git init(and then add files to .gitignore to ignore the files)


