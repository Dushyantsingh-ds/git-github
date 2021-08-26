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

# Practice Time

How to implement git in our project.

### Step-1 initialization

- Open Git Bash in your working Dir. using Right click on the folder and select Git Bash.

- type ``` git status ``` & hit the enter 

- output ``` fatal: not a git repository (or any of the parent directories): .git ```

its means there is no any git initialized.

- type ``` git init ```

- output ``` Initialized empty Git repository in D:/Learn/Git/.git/ ```

now your working directory have a git file.

- type ``` git status ``` & hit the enter 

-output (I have 4 file in my demo project)

``` On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ExcleFile.xlsx
        NoteFile.txt
        WordFile.docx
        new%file.txt

nothing added to commit but untracked files present (use "git add" to track)
 ```
 
 ## Step-2 Add file from Working Dir to Stagging Area.

- type ``` git add . ``` & hit the enter // if you want to add all file or spacific you can use ``` . ``` Or ``` --a ``` OR ``` NoteFile.txt ```

- type ``` git status ``` & hit the enter 

output

``` 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   ExcleFile.xlsx
        new file:   NoteFile.txt
        new file:   WordFile.docx
        new file:   new%file.txt

```
Color Diffrance Red to Green (Red means Your file is tracking not in Stagging area. or Unmodify & Green Means you file is add into Stagging area with Modiifide)

### Step-2 Commit your file

- type ``` git commit -m "First Commit" ``` & hit the enter 

- output

```
[master (root-commit) 9c6946c] first Commit
 4 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ExcleFile.xlsx
 create mode 100644 NoteFile.txt
 create mode 100644 WordFile.docx
 create mode 100644 new%file.txt
```

- type ``` git status ``` & hit the enter 

- output 

``` 
On branch master
nothing to commit, working tree clean

```

Congrats you have successfully implement git in your project.

## Step-4 See the Commit information

- type ``` git log ``` & hit the enter 

- output

```
Author: Dushyant Singh <dushyantsinghxxxxx@gmail.com>
Date:   Fri Aug 27 03:38:59 2021 +0530

    first Commit

```

XXXXXXXXX End of Praticle  XXXXXXXXX
