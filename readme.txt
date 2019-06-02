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

