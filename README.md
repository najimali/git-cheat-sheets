# Git Cheat Sheet for beginners
Basic commands
1. init - initialize the local git repo
2. git add<file> - add files to staging area
3. git status - check status of working tree
4. git commit - Commit changes in staging area
5. git push - Push to remote 
6. git pull - Pull latest from remote repo
7. git clone - Clone remote repo locally
8. git branch <branch _name_1> - Create a new branch
9. git  checkout <branch_name_1> - Switching to branch
10. git rm --cached file_name  - to remove the file

Prequistic
1.Editor - VS code
2.Gitbash - https://git-scm.com/downloads
3.Github accounts 
Different method to create files 
1. file_name 
eg git add index.html - it will add the index.html file only
2. star(*)
eg - git add *.html - it will add all the html files
3. directory(.)
eg - git add . - it will all the files in the directory 
Note - git add . is most common way of adding files.

Commit in git
1. git commit - then a window will pop then add your msg
2. git commit -m  "Add your message here" (Note - use double quotes when terminal is cmd & single quotes when git bash is used)

Clear the terminal - 
For window
command - cls
For git bash
command - clear 


Check latest commit 
command - git log
 O/p format - 
 1.comimit id
 2.Author: name <email>
 3.Date: Mon June time
 
 4.Commit Message
 
Checking out w.r.t id 
command - git checkout 10-15 first char of the id

Note - After using git chechout we won't see all those commit or changes in the file which are done after this id
so use to go back to previous use 
-git checkout master 


How to ignore files ??
create a file with extension .gitignore
then add the all the file name in the gitignore then git won't keep track of these file


for eg we have file_1.txt ,file_2.js,file_3.hmtl
Now add these file in ignore file 
file_1.txt
file_2.js

any changes made in file_1 & file_2 will not be tracked
to check this use git status

Branching in Git
Initially we are in master branch & suppose you want to change something in one file then you create your branch first then edit in that branch then merge
Note - Don't directly do changes in master branch
Create a new branch
commad - git branch branch_name_1

Switch to any branch 
command - git checkout branch_name

How to create new branch & switch to it in one line ??
command  - git checkout -b new_branch_name (-b means you created a new branch)
if already branch is created then use command - git checkout branch_name Connect Git with github

Posting your code on github
Go to github 
create a new repo & then copy the repo link

then in the terminal
git remote
git remote add origin repo_link
git push -u origin master
 

 
 Merge the two branch
 create a new branch using - git checkout -b branch_1
do your collabrartion in the branch_1 
the switch to master branch using command- git chechout master
merge them using  - git  merge branch_1


How to collabrate in others project 
1. make a clone of others repo using - git clone repo_link
2. make a separate branch using - git checkout -b new_branch_name
3. Do collabration by adding new file or modify existing one 
  a. make the changes
  b. add all the changes =>  git add . & add commit =>git commit -m'Your commit message'
4. switch to master branch - git checkout  master
5. merge them => git merge branch_name
6. push them on the github using - git push 
7. then second developer will see chnages you made by using git pull
