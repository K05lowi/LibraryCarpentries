# Introductory teaching in the relationship between Git & Github
This introduction covers the basics of what Git and GitHub are, the concepts and the basic commands. Bring attention to that the terminology
is different in Git and GitHub.

During teaching Git and the folder we are working in (on our path finder) are both open. This shows that when you fx create a file in Git,
the file now exists on your computer. Likewise, when a file is deleted through Git, it is deleted in from the folder on your computer.

## Pedagogy
* Begin by drawing on the board the Git workflow on your own comupter
* Show basic functions in Git (hands on)
* Draw and explain branch function (still on own computer)
* Show Branch (hands on)
* Draw Github and draw in with arrows relation to GIT
* Hands on in making a GIThub repository and pushing files to the repository

## About Git
Git is a version control system for tracking changes in computer files. Many people can work on thesame project together and all changes to the project
will be tracked. You can reverse back to a version of any tracked file at any time, as long as the file has been commited (saved) to the your repository (project folder).

When you use Git you have a master copy of your project. It is best practice to make a copy of your project (a branch) and work on that branch, only adding merges (updates) to your master when you are sure about them. This is good practice - do not mess with your base data!! When you are finished working locally on your computer and want
to share your work in a collaborative space outside of your own computer environment, such as an online remote repository like GitHub, you PUSH your files frolm your computer to the remote repository. On the remote repository you can accept the changes to the files and merge them into a project so everyone can see your work (or reject your work!)

## The Concept of git
In git your create, delete and add content to your files. When you are satisfied your files are ready to be saved, you ADD them to a staging area and then
save them using the COMMIT command. When files have been commited, you can go back at anytime to see changes to the files and revert back to these changes.

## Git commands
**git init** initializes a .git repository on your computer which is hidden by default. Go into the folder settings options (in your path finder) and under the general tab, unhide hidden files.

**git add** adds files to staging area and then they are ready to commit. Run this action as many times as you need before saving (committing) and it will keep the
files in the staging area

**git status** check the status of your work. Shows you the differences between what is being committed and what you have in your folder, but not worked on or have not
chosen to add to the staging area (ie maybe you have forgotten something?)

**git commit** saves your changes into your local git repository

**git push** takes your local git repository and sendes everything to the remote repository you have assigned as the place you will share your work with your group.

**git pull** pulls out the latest changes from the remote repository down to your local copy on your computer. This practice means you always have the most up to date
version of the project to work on.

**git clone** Make a copy a remote repository 

## Workflow
* Create a folder on the desktop
* Right click and open in Git Bash
* create 2 files: touch app.txt and touch index.html
* Add content to one of the files
* ls
* git init
* git config --global user.name
* git config --global user.email
* git config --list
* git add filename (to add your files to the staging area)
* git status
* git rm --cached (remove files from staging area but not delete from folder)
* git add *.txt (to add all text files, this can be done with all formats such as *.html)
* git add . (to add all files)
* edit a file and save
* git add .
* git status
* git commit (fill out a commit message, use CTRL+X to quit the message if necessary)
* git status
* edit a file and save
* git add .
* git commit -m "write commit message"

## Introduce version control
* git log --oneline (this shows you the commit message ie the changes you have made and when. Note the commit ID)
* git show filename (will show you the history of the document)
* git checkout commitID filename (to revert to previous version of a document)
* git status 



## Discussion points
The Git respository file (master) you create on your computer is by default hidden.

## Diagram
