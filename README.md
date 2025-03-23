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

Push locally created branch to remote location
=================================

git remote add origin "link of git remote repository "
Git remote, now remote mean somewhere else, but not on this computer. We're  going to use this to add a reference to the remote  
repository on GitHub.

git remote -v 
============
 it shows any remote repositories that I've connected to this repo.

 git push -u origin master
 ================
 u - upstream
 meaning this is where I want to push it to  by default. So I'm going to do dash u for set  
upstream and then enter In the future, I can just  use git push without typing out origin Master

Git Branching stratagey 
===========================
Master or Main Branch 
Development Branch 
hot fix branch 
feature branch 
Release Branch 

Master brnach
Now master is a naming  convention for the main or the default branch in  a repository. So if you're just working off of one  branch, that's where your code will live, and all  
your code, all your commits, everything will be  in that one branch. Now, this is called branching,

feature Branch

this  new feature branch will be exactly the same. But  as you make updates to the feature branch, those  changes are only seen in the feature branch. So if  
you make changes on the feature branch, you make  a commit to save those changes on to that branch.  
And then you switch back to the master branch, you  won't be able to see any of the changes that you  made on that feature branch. 
Each individual  branch has no way of knowing what commits or
what changes have been made to any other branch.  Each branch is only keeping track of what changes  
are made on its own branch. Now you can continue  to change the code on master branch and save it 

Why is this useful? 
============
extremely useful because you will be building out  new features to applications that may break your  code or they are not finished yet. And you don't  want to save them to the main master branch. You  
want to work on them in kind of a sandbox area. So  you can write all the code unit And get it correct  and in the state that you want, before you merge  it back into the main branch of the code base.  
And this is really helpful when you have many  different people working in the same repository,  or a lot of different branches going on at  once.

scenario
==========
One very common thing that you'll see  in development is that you'll be working on let's  say, this feature branch for a week or more, and  you have all of these changes that you've made.  And then you find out there's this major bug that  you have to fix real quick. So for that, we make  this other branch called a hotfix branch here, represented by yellow. And you can see that I made  the change in one commit to fix whatever bug was  wrong with the code on its own branch, I made sure  it was working correctly. And then I merged it  back into the master branch. 
