Read me file:
=============
This is a demo repo created to practice certain basic commands. I am logging certain commands here.
a) First sign in to git hub account
b) click on "new" to crete a new repo
c) you can optionally add readme file automatically or after creating new repo you can manually create readme file. - its a markdown file
  the purpose of readme is to create general information that is relevant to the project. say name of the project, short description, some important initial info ,etc
d) once you finish typing click on commit changes button
e) after commit you can see the readme file along with commit msg. in case you need to edit or view, click on that readme.md link and you can view then click on pencil icon to edit. after editing click on commit changes and give commit text so that we track the history of changes and its reason. this stands the same for all kind of files that you upload

setting up of git in local:
============================
To find the version of git or to check if git has been installed: git --version on your local vs code terminal or the local command prompt
To install git on to your local: https://www.atlassian.com/git/tutorials/install-git?section=windows
Why to install git on local: you need to map to to the cloud repository. you must execute all git commands. you are constantly going to work on local and make changes to cloud repo. so you need to install for mapping your folder with git repo

Code Editor:
============
You need code editor like visual studio for writing down code.
even this can do some mapping and exectue commands on git
install vs code - editor - from code.visualstudio.com - used by professionals - free of cost- (you can even use simple notepad, wordpad but not recommended for huge projects)

In code editor, 
a. you can always use terminal and use git commands to interact with repo
b. alternatively there would be certain options in vs code itself to interact with repo

Mapping of local folder and git repo:
=====================================

Now we can do 2 things - not something related to code editor but about mapping the local with git repo
Way 1. clone the repo that is created on git hub clouds and map it to the local - you first take the base from repo and map it to local
Way 2. add the local repo to git hub clouds repo - you want to add something which is local and add to repo

Way 1: clone the repo to local
1) create a folder and add that to vs code
2) goto terminal and use the command: git clone ssh link here   (to get ssh link goto github repo -->click on clone for download-->copy ssh id and complete the command execution on the terminal
git clone git@github.com:Sudhavalli1106/practicematrimorphosis.git
 for this you need to authentiate ssh
3) alternatively you can add https for clone
if everything is successful, the cloud folder or files get downloaded to local.

How to find .git folder or is your folder got the clonned files from repo?
==========================================================================
now when you see vscode on local, your git folder looks very normal like others. how can you know if the folder is git-enabled? you can go to that file location you see a hidden file ".git" which indicate that its mapped to git.
alternatively you can use command to list all the files. use ls -force on windows to show all files including hidden file.

Git commands:
=============
1. git status : this will show all changes between local and cloud. this will show modified and utracked file
     modified - file is existing on both local and git repo and there is a change
     untracked - a file that is available on local but not on git repo cloud
   so for untracked to be tracked -> so first the files that are in local to be added to git repo. use "add" command
   command: git add .   (. represent all files that are untracked to be tracked)
   command to add specific file: git add index.html
2. git add filename or git add .
  after adding you can always use git status to check if this is mapped with git folder on local
  it will be into staging now. but unless you say commit, these will not be added to clouds. now at present is on local git. so you have to commit
4. git commit -m "reason for commit" -m "reason you can give here in detail way"   (similar to dialog box that you got while you commit directly on git cloud)
5. 
