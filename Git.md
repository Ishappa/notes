 
 
 
 # Initialize Git repository if not already done
git init

# Add remote repository
git remote add origin https://github.com/username/repo-name.git

# Stage all changes
git add .

# Commit the changes
git commit -m "Initial commit"

# Push to the main branch
git push -u origin master

 
 or if you are pushing code to new repo
==============================================
1. Go to your GitHub account settings.
2. Navigate to Developer settings > Personal access tokens.
3. Click Generate new token.
4. Select the scopes you need (e.g., repo for full control of private repositories) and generate the token.
5. Copy the token. This will be used in place of your password.
6. Update the Remote URL:

 command example: 
 -----------------
 
	git remote set-url origin https://Ishappa:<your_personal_access_token>@github.com/Ishappa/JavaScript-New.git
	
	

Push Change
--------------

git push -u origin master
 
 
 # for existing repo with code
 
 1. git clone repoUrl           (it will pull all data)
 
 after modified the any code 
 
 # Stage all changes
git add . or git add --all

# Commit the changes
git commit -m "Initial commit"

# Push to the main branch
git push -u origin master


 
 vscode git push all data changes
 ===================================
 
 codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git branch
* local
  main
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git push -u origin local
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 579 bytes | 579.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/IshappaN/demo1.git
   d208750..0adf30b  local -> local
Branch 'local' set up to track remote branch 'local' from 'origin'.
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ 
 
 
 
 Commads using in GitBash (search in startmenu)
==========================
git add -help    				 (will display all posssible add related commands -->traking)
git commit -help   				(will display all posssible commit commands)
git help --all  				(will display all posssible commands)


Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ whoami							-->showing username
Ishwar		

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ pwd								--->showing current working directory name (/c/Users/Ishwar)
/c/Users/Ishwar

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ ls								--->This cmd will show all folders and files in current directory
'3D Objects'/
 AppData/
'Application Data'@
 Contacts/
 Cookies@
 Desktop/-----etc
 
Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ cd desktop							--->This cmd will change the current directory working path to desktop  (/c/Users/Ishwar To Desktop)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop	
$ pwd								--->present directory is changed
/c/Users/Ishwar/desktop	

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop
$ mkdir git_project						--->This cmd will create the new directory (now its creating git_project folder in desktop )

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop
$ cd git_project						--->This cmd will change the Desktop directory working path to git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ cd ..					 			--->This cmd is used for go to the previous Directory (it will go to git_project to desktop)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop
$ cd git_project						--->again its chnaging desktop to git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ touch newFile.txt						--->This cmd will creating the file in git_project(touch)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ pwd								--->showing current working directory
/c/Users/Ishwar/desktop/git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ ls
newFile.txt							--->showing all files in current working dirctry

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ echo This is some text in second file >secondFile.txt		---> this is creating second file with writing some text inside that file (echo)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ echo this is new file >newFile.txt				---> this is writing some text inside new file 

============================================================================

GIT CONFIGERATION :
------------------------
Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ git config --global user.name "Ishwar N"			--->Set the username  
										(global keyword is for set our username and email in evry repo in our device)
Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ git config --global user.email "ishwarkuri4@gmail.com"	--->Set the email 

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ git config --list						--->list of configeration (showing in the last lines)
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=Ishwar N
user.email=ishwarkuri4@gmail.com

=========================================================================

GIT INITIALIZATION : open GitBash
-----------------------------------

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ pwd										-->showing present drctry
/c/Users/Ishwar

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ cd desktop									-->changing /c/Users/Ishwar To desktop


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop
$ mkdir git_project								-->created git_project foldr in desktop

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop
$ cd git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project
$ git init									--->(git init) is used for initialize the git
Initialized empty Git repository in C:/Users/Ishwar/Desktop/git_project/.git/

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)

===============================================================================

GIT STATUS: 
-----------------
Created demo file in vs code in the git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ ls										--->showing files in the folder
Demo.java


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status									--->this cmd will check the status of the file(Tracked or Untracked)
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)		 
        Demo.java

nothing added to commit but untracked files present (use "git add" to track)


GIT STAGING (STAGING FILES) :
----------------------

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git add Demo.java								-->for make tracked file use this cmd

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status									-->no untracked files and its asking for commit the file
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Demo.java



Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Demo.java

Changes not staged for commit:						-->(I modify or added few code in the demo.java file without commit the file bcs its showing this msg )
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Demo.java



Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git restore Demo.java							--> for restoring the previous data to the file and deleted the modifyed data 

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Demo.java

STAGING MULTIPLE FILES:
-------------------------

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git add --all    							-->add or make tracked files or use (git add --all or git add -A) can use any one cmd

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   Demo.java
        new file:   Index.java

 


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git commit -m "first version chnages in Index and Demo"			-->this cmd is used for commit the staging files we should pass msg
[master (root-commit) 14e6c3d] first version chnages in Index and Demo
 2 files changed, 12 insertions(+)
 create mode 100644 Demo.java
 create mode 100644 Index.java


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status									-->status of the files
On branch master
nothing to commit, working tree clean


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git status									-->status of the after modify the commited files 	
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Index.java							-->git status --short(this cmd will display shprt msg  ex:M -->for modified files)

no changes added to commit (use "git add" and/or "git commit -a")



Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)    
$ git commit -m "hrlo"					-->Once we modifyed the commited file we need to add/stage and then commit else it will tell us staged the files
On branch mastepwdr
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Index.java

no changes added to commit (use "git add" and/or "git commit -a")



Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git commit -a -m "second modify chngaes"                             --->shortcut cmd for the add and commit the files(stage and commit)
[master 42d372e] second modify chngaes
 1 file changed, 1 insertion(+)

Git Branch:
-------------------------

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ pwd
/c/Users/Ishwar

Ishwar@DESKTOP-CRRF53D MINGW64 ~
$ cd Desktop

Ishwar@DESKTOP-CRRF53D MINGW64 ~/Desktop
$ cd git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/Desktop/git_project (master)
$ git branch new							-->created a branch(new)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/Desktop/git_project (master)
$ git branch
* master
  new

Ishwar@DESKTOP-CRRF53D MINGW64 ~/Desktop/git_project (master)
$ git checkout 'new'                                             -->chnage the branch loc
Switched to branch 'new'
M       Demo2.java
Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ ls
Demo1.java  Demo2.java  out/

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git checkout new
Switched to branch 'new'

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (new)   --->here is a 3 files in new branch
$ ls
Demo1.java  Demo2.java new.txt  out/

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (new)
$ git checkout master
Switched to branch 'master'

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git merge new							--->its is use for merge new branch to master then all files merge into master															

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ ls
Demo1.java  Demo2.java  new.txt  out/

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git branch -d new                                           --->this is for delete a specifuc branch(ex: deleeting new branch)

GIT HUB::
===========

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop
$ cd git_project

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git remote add origin https://github.com/Ishappa/Hello-Git.git                 -->adding files into newly created repo in github(specify the link fron github)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project (master)
$ git push --set-upstream origin master						--->pushing all files to Hello-Git repo from master branch
info: please complete authentication in your browser...
Enumerating objects: 26, done.
Counting objects: 100% (26/26), done.
Delta compression using up to 8 threads
Compressing objects: 100% (22/22), done.
Writing objects: 100% (26/26), 6.72 KiB | 1.34 MiB/s, done.
Total 26 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), done.
To https://github.com/Ishappa/Hello-Git.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.


README.md --> this file used to pass some text messsage about our repo we edit or update in github.

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git pull orgini					 --> for pull all files from git(README.md)

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git push origin					 --> for push all files to git if we edited somthing (1st we need to do stag and commit)


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git log origin/master								-->this is used to display all chnages in files.check upto date chnages in our files
commit 3e4bb11f9a76dd7b1b10a68942f5ba10bc5b8a36 (HEAD -> master, origin/master,
branch1)
Author: Ishwar N <ishwarkuri4@gmail.com>
Date:   Mon Jan 29 12:58:53 2024 +0530

    commited 3 files included txt

commit 0d64987a172b7f4e66394af264a58c0549585973
Author: Ishwar N <ishwarkuri4@gmail.com>
Date:   Mon Jan 29 12:34:54 2024 +0530

    commited two files

commit f443a2c4be724fce4c6fd30c82130a2286fe266e
Author: Ishwar N <ishwarkuri4@gmail.com>
Date:   Mon Jan 29 12:28:37 2024 +0530

    demo1 is commited

-----------------------------------------
Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git branch -d branch1                            -->this cmd is used to delete a branch(branch1-->branch name).


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git pull						-->this is used to pull all our newly created branch form git to local.
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 953 bytes | 35.00 KiB/s, done.
From https://github.com/Ishappa/Hello-Git1
 * [new branch]      new-Hello-Git1-branch -> origin/new-Hello-Git1-branch				<--
Already up to date.

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git branch
* master			-->still it is not showning our newly created(new-Hello-Git1-branch) git branches in local.


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git branch -a					-->is used to display all branches in local after pull
* master
  remotes/origin/master
  remotes/origin/new-Hello-Git1-branch
			
Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (master)
$ git checkout new-hello-git1-branch				-->this is for swith our master branch to new-hello-git1-branch.
Switched to a new branch 'new-hello-git1-branch'
branch 'new-hello-git1-branch' set up to track 'origin/new-hello-git1-branch'.

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (new-hello-git1-branch)
$ git checkout -b updating-readme					-->this cmd is used to create and switch to newly created branch
Switched to a new branch 'updating-readme'


Then you can modified something in readme file in your local because it is already pulled all files from new-hello-git1-branch(Git Hub).
after edited you have to staging and commit normal process 

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ git add README.md

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ git commit -m "somthing is chnged and commited"

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ git push origin updating-readme  			-->this is for push our README.md file to git 
							but brnch will be updating-readme you can compare merge README file to orginal/other branches.


Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ git log --oneline                                         		 -->this cmd will be check all commit chnages in our repo lastest will be 1st.

f7798e8 (HEAD -> updating-readme, origin/updating-readme) somthing is chnged and commited from local on git readme.md file
5288e13 (origin/new-Hello-Git1-branch, new-hello-git1-branch) Update README.md
c61442a (origin/master) modified readme file
ef348ca Update README.md
a386fd7 new added demo3 file
33edffc Update README.md
ede6cb3 Create README.md
3e4bb11 commited 3 files included txt
0d64987 commited two files
f443a2c demo1 is commited

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ git reset 33edffc						-->we can filter by reset based on id
Unstaged changes after reset:
M       README.md

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ git log --oneline						-->filterd output
33edffc (HEAD -> updating-readme) Update README.md
ede6cb3 Create README.md
3e4bb11 commited 3 files included txt
0d64987 commited two files
f443a2c demo1 is commited

=================================
Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
$ touch .gitignore						-->is used to create file(created .gitignore) whenevr want to hide some files.

Ishwar@DESKTOP-CRRF53D MINGW64 ~/desktop/git_project1 (updating-readme)
git clone https://github.com/Ishappa/Hello-Git1.git   		-->is used copy the git project to our local folder


MARKDOWN HEADINGS(profile setting ->scroll up last option--> check ok for markdown edit)
==============================================================
# larger for heading
## medium font for heading
### small font for heading

text decoration:
==============
**sjkcbscjslk**				-->make a bold.
*skjbcscsskdm csl*			-->italic.
***ksjbckwjjcnakln***	 		--> bold italic text.
**acbajscbclk_jskc_sacjnalkcn** 	-->bold with italic only specific txt(jskc).
~~wljncwlkcn~~ -->text decorate:line will be on text(scratch text).



Make a paragraph as looks like Quote.(> with space starts of paragraph)
========================================================================
Ex:

> In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate 
Lorem ipsum may be used as a placeholder before final copy is available

Making a Nested Quotes structure:
=================================
Ex: 

> In publishing and graphic design, Lorem ipsum is a placeholder text commonly used to demonstrate 
Lorem ipsum may be used as a placeholder before final copy is available
>
>> Lorem ipsum may be used as a placeholder before final copy is available

Lists(giving space is import after symbels)
======
1. one
2. two

for bulletpoints
- one
- two

bullet points with quotes 
* one
> hello evryone
* two

making code blocks
===================

***        --> is to ccreate horizontal line

```html--> for make strucrture a html code and copy .
1. ONE

<html>
<head>
<title>This is 1st title</title>
</head>

2. TWO

<html>
<head>
<title>This is 2nd title</title>
</head>

3.


Links and URL
=============

my fav search engine is [Google](https://www.google.com "this is so useful") makes link.

<https://www.google.com> ---->makes url
