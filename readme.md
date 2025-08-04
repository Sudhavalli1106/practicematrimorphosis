Read me file:
=============
git hub helpful video:  https://www.youtube.com/watch?v=RGOj5yH7evk

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

Way 2: clone local folder to new repo:
1) create a folder on the vscode
2) use git init so that it creates .git folder
3) create the necessary files
4) create new repo on the git
5) now we need to map local to cloud repo: use command => git remote add origin "give ssh here"

   
How to find .git folder or is your folder got the clonned files from repo? - more detail info
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
commit will commit locally only. it wont update the cloud
5. git pull origin main => pull the changes from cloud to local
6. git push origin main => will push the local committed changes to cloud


suppose you have 1st line which you want from local and you have line 2 from git and you want to accept.

git add .
 
git rebase --continue 
resolve conflict
git push

**
Steps for multiple addition, modification and deletion**

# 1. Stage your changes
git add .

# 2. Commit locally
git commit -m "Your local changes"

# 3. Pull with rebase to handle conflict
git pull --rebase origin main

# 4. When conflict appears, edit the file:
#    - Keep line 1 from local
#    - Keep line 3 from remote
#    - Save file

# 5. Stage resolved file
git add <filename>

# 6. Continue rebase
git rebase --continue

# 7. Push changes
git push origin main

**What is staging and unstaging?**
**Staging:** you use "add" to staging meaning it is ready to be committed. only commited changes can be pushed
**unstaging:** you use "reset" to unstage. these can't be committed. its like a file is not ready to be staged
**restore**: git restore filename - its like undoing file changes on local**
suppose after a commit you want to unstage:**
reset: You can reset 


