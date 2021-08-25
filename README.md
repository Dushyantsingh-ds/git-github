## KeyPoints
- Pull : 
getting file, Data from server into our System/Locally
- Push : 
Send/Tranfer My file/Data to main server or main Presental Location/Server/Repo.


## What is Git
Git is a free, open-source version control software. It was created by Linus Torvalds in 2005. 
-This tool is a version control system that was initially developed to work with several developers on the Linux kernel.
-It takes Snapshot of the changes.

## Two Type of System 
Centralized and Distributed

### Centralized :

Cons: Only One Repo available for everyone, If you change anything that will affect the whole repo, No any personal old cahange record.

### Distributed : 

Pros: -Every one can clone main Repo, That clones repo, makes his/her own personal repo. 
When he want to do any chanage in the local repo, that change will not affact main/prasental repo with permit the Ower of the presental repo.
-Having all his/her personal old cahange record.
-Everyone having Whole project that he cloned.

Available tools for mangesning free Git use : Github, GitLab, GitBucket

# Features

## SnapShoot: 

It takes the snapshoot of the changes. like a photo shoot


## CheckSum : 

CheckSum is a techqun to see our data tranfer protected or un protected. Every Data/File having own diffrent CheckSum in the form of String. 

# Install Git using : 
Visit offical site: https://git-scm.com/downloads 

If you already have Git installed, you can get the latest development version via Git itself: 
``` git clone https://github.com/git/git ```

# Commands Basics

``` Git Status ```
// is used to check the sitution of the repo. or workload.

``` Git init ```
// is used to initialized/create repo. of  your folder in '.git' hidden folder.

``` Git add --a ``` OR ``` Git add . ``` OR ``` Git add FileName.Txt ```
// is used to add the file from Working Directory to Stagging Area

 ``` Git commit -m "Commit Title" ``` 
// used to commit your changes, or to send files from Stagging Area to Repo.

 ``` Git log ```
// to see the all changes detial, Who had, DateTime, UserName....

