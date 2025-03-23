Git 
====
Version control is  basically a way that we as programmers track our code changes,

What is version control?
================
 we basically save an initial version  of our code into Git. And then when we update  
code, we can save it into Git again, and again and  again and again. And throughout time as our code  
continues to change, we can look back at all of  the changes we have made over time. This helps us  
to see and understand what we did when, as well as  track down bugs, or go back to a previous version  
of the code if we need to.

repo -> repository
project or the folder place where your project  is kept. You can call it a repository.

READ.md -readme.md for markdown. markdown is basically  an easy way to format your text in these sort of  
files.

Git VS Git Hub
===========
 Git  is the tool that tracks the changes in your code.
GitHub is a website where you host all  of your Git repositories. Being online, it makes  
it easy to work in groups with other people, and  organize your projects into a portfolio for you to  
show potential employers

Git Commands 
=============
clone -> bring a repo down from the internet (remote repository like Github) to your local machine

add -> track your files and changes with Git

commit -> save your changes into Git
 git commit
 git commit -m
 M is for message
 you need to have a  message in order to commit your files. 

push -> push your changes to your remote repo on Github (or another website)

git push 
git push origin master

origin - origin is an option set for us  here, and is basically a word that stands for  
the location of our Git repository.

Master - is the  branch that we want to push to

pull -> pull changes down from the remote repo to your local machine
When there  are changes to your code on GitHub, and you want to bring those to your local machine, then you use  the pull command, you pull down changes from the  
remote repository.

status -> check to see which files are being tracked or need to be commited

init -> use this command inside of your project to turn it into a Git repository and start using Git with that codebase

To Check Version
===============
git --version

Initialize Git
--------------
git init
To create a new repo, you'll use the git init command. git init is a one-time command you use during the initial setup of a new repo. Executing this command will create a new . git subdirectory in your current working directory.
.git file will be created - hidden files

git status
========
git status
the git status command shows me all of the files that were  updated or created or deleted,

git add 
==========
to track the file before you can save it to get  to do that, you need to use the git add command,  
and then tell it which files to track. 

git add .
========
Now most of  the time, or a lot of the time you see people use  a period, which means you're telling Git to track  all of the files that are listed here, 

