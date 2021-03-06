# Git & GitHub 
## KeyPoints
<details>
  <summary>Click to expand!</summary>
 - Author :
  who creates the file
  
  - Commit :
  who update/delete the file but not create.
  
- Pull : 
 getting file, Data from server into our System/Locally
 
- Push : 
 Send/Tranfer My file/Data to main server or main Presental Location/Server/Repo.
</details>

# About
<details>
  <summary>Click to expand!</summary>
## What is Git
<details>
  <summary>Click to expand!</summary>
Git is a free, open-source version control software. It was created by Linus Torvalds in 2005. 
-This tool is a version control system that was initially developed to work with several developers on the Linux kernel.
-It takes Snapshot of the changes.
</details>

## Two Type of System 
<details>
  <summary>Click to expand!</summary>
 Centralized and Distributed
 
### Centralized :

Cons: Only One Repo available for everyone, If you change anything that will affect the whole repo, No any personal old cahange record.

### Distributed : 

Pros: -Every one can clone main Repo, That clones repo, makes his/her own personal repo. 
When he want to do any chanage in the local repo, that change will not affact main/prasental repo with permit the Ower of the presental repo.
-Having all his/her personal old cahange record.
-Everyone having Whole project that he cloned.

Available tools for mangesning free Git use : Github, GitLab, GitBucket
</details>
</details>

# Features
<details>
  <summary>Click to expand!</summary>
 
## SnapShoot: 

It takes the snapshoot of the changes. like a photo shoot


## CheckSum : 

CheckSum is a techqun to see our data tranfer protected or un protected. Every Data/File having own diffrent CheckSum in the form of String. 
</details>

# Setup
<details>
  <summary>Click to expand!</summary>
  
## Install Git using : 
<details>
  <summary>Click to expand!</summary>
INSTALLATION & GUIS
 
With platform specific installers for Git, GitHub also provides the 
ease of staying up-to-date with the latest releases of the command 
line tool while providing a graphical user interface for day-to-day 
interaction, review, and repository synchronization.
 
Visit offical site: https://git-scm.com/downloads 
 
GitHub for Windows
 
htps://windows.github.com
 
GitHub for Mac
 
htps://mac.github.com
 
For Linux and Solaris platforms, the latest release is available on 
 
the official Git web site.
 
Git for All Platforms
 
htp://git-scm.com


If you already have Git installed, you can get the latest development version via Git itself: 
``` git clone https://github.com/git/git ```
</details>
 

## User SETUP cmd
<details>
  <summary>Click to expand!</summary>

Configuring user information used across all local repositories

``` git config --global user.name ???[firstname lastname]??? ```

set a name that is identifiable for credit when review version history

``` git config --global user.email ???[valid-email]??? ```

set an email address that will be associated with each history marker

``` git config --global color.ui auto ```

set automatic command line coloring for Git for easy reviewing

</details>
</details>

# Git Commands >>>>
## vim text editor
<details>
<summary>Click to expand! </summary>
### i // used for insert 
  ### Esc // exite from typing area, come from command area
  ### :wq // to save the changes in vim
  </detials>
## Quick Commands
<details>
<summary>Click to expand! </summary>
### q // exit from commands  
### rm -rf .git // used to delete the repo.
### git log -p // see the logs with the change in content *
### git log -p -3 // see the logs with only 3 top commits diit in content *
### git log --stat // see the oeverview of commits in summary *
### git log --pretty=oneline // to see the all commits title  *
### git log --pretty=oneline // to see the all commits title with author. 
### git log --since=2.days // to see the commits of 2 days before *
### git log --since=2.weeks // to see the commits of 2 week before *
### git log --since=2.months // to see the commits of 2 months before *
### git log --since=2.years // to see the commits of 2 years before *
### git log --pretty=formate:"%an -- %ae // to see the all author with his/her Hass "%an= author name and %ae = author email 
### git log --pretty=formate:"%h -- %an // to see the all author with his/her Hass "%h= hass and %an = authorname for more log commands visit : git-scm.com/docs/git-log
  



</details>

## Working Commands
<details>
  <summary>Click to expand! </summary>
## STAGE & SNAPSHOT cmd

<details>
 Lev.1 <summary>Click to expand! </summary>
 
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

</details>

### @Practice Time 


<details>
  <summary>Click to expand!</summary>
 
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
</details>
  
## IGNORING PATTERNS
<details>
  <summary>Click to expand!</summary>
 
Preventing unintentional staging or commiting of files

``` 
logs/
*.notes
pattern*/
``` 
Save a file with desired paterns as .gitignore with either direct string
matches or wildcard globs.
  
``` git config --global core.excludesfile [file] ```
  
  system wide ignore pattern for all local repositories
</details>
 
 ### @Practice Time 


<details>
  <summary>Click to expand!</summary>
 
How to implement .gitignore in our git project.
 
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
## Step-2 Add file a new file, In my case i create a .log file in my project.
 
 ``` touch system.log ``` // this command is used to create a file
## Step-2.0 check status
 ``` git status ```

 output 
 
 ```
 $ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        system.log

nothing added to commit but untracked files present (use "git add" to track)
```
 
## Step-3 Create a .gitignore file
 
  ``` touch .gitignore ``` // this command is used to create a .gitignore file

 ## Step-3.0 check status
 ``` git status ```

 output 
 
 ```
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        system.log

nothing added to commit but untracked files present (use "git add" to track)
``` 
## Step-4 Add file name or dir name that you want to untrack or unuse in git
 
 -Open .gitignore file in any text editior and type the file or dir name
 
 - as file name : ``` system.log ```
 - as dir name : ``` dir_name/ ```
 - as a extension : ``` *.log ```
 
 -if you want to track only one dir.
 - as sub dir : ``` /dir/ ```
 - as dir : ``` assets/dir/ ```  & save the file


 ## Step-3.0 check status
 ``` git status ```

 output 
 
 ```
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
```
 
## Step-5 Add file from working dir to Stagging Area.
- type ``` git add . ``` & hit the enter // if you want to add all file or spacific you can use ``` . ``` Or ``` --a ``` OR ``` NoteFile.txt ```

- type ``` git status ``` & hit the enter 

output

``` 
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
```
 
Color Diffrance Red to Green (Red means Your file is tracking not in Stagging area. or Unmodify & Green Means you file is add into Stagging area with Modiifide)

### Step-6 Commit your file

- type ``` git commit -m "First Commit" ``` & hit the enter 

- output

```
$ git commit -m "first commit"
[master (root-commit) 90899bd] first commit
 5 files changed, 283 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 ExcleFile.xlsx
 create mode 100644 NoteFile.txt
 create mode 100644 WordFile.docx
 create mode 100644 new%file.txt

```

- type ``` git status ``` & hit the enter 

- output 

``` 
$ git status
On branch master
nothing to commit, working tree clean
```

Congrats you have successfully implemented .gitignore in your git project.

## Step-4 See the Commit information

- type ``` git log ``` & hit the enter 

- output

```
commit 90899bd4d21271b67f75743c5d17e9e11b5fcfa5 (HEAD -> master)
Author: Dushyant Singh <dushyantsinghxxxxx@gmail.com>
Date:   Fri Aug 27 18:12:17 2021 +0530

    first commit


```

XXXXXXXXX End of Praticle  XXXXXXXXX
</details>
 
  ## Git diff: see the differences.
<details>
  <summary>Click to expand!</summary>
 
 ``` git diff``` 

diff of what is changed but not staged OR see diff between tracked and staged

``` git diff --staged ``` 

diff of what is staged but not yet committed OR see diff between staged and committed 

</details>
  
 
  ### @Practice Time 


<details>
<summary>Click to expand!</summary>
 
How to implement .diff in our git project.
 
### Step-1.0 initialization

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
        .gitignore
        ExcleFile.xlsx
        WordFile.docx
        new%file.txt
        system.log

nothing added to commit but untracked files present (use "git add" to track)

 ```

## Step-1.1  Add file from working dir to Stagging Area.

- type ``` git add . ``` & hit the enter // if you want to add all file or spacific you can use ``` . ``` Or ``` --a ``` OR ``` NoteFile.txt ```

- type ``` git status ``` & hit the enter 

output
 
 ```
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .gitignore
        new file:   ExcleFile.xlsx
        new file:   WordFile.docx
        new file:   new%file.txt
        new file:   system.log
```
 
### Step-1.2 Commit your file

- type ``` git commit -m "First Commit" ``` & hit the enter 

- output
 
 ```
[master (root-commit) 326e677] First Commit
 5 files changed, 191 insertions(+)
 create mode 100644 .gitignore
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
  

 ## Step-3.0 check status
 ``` git status ```

 output 
 
 ```
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)
```
  
## Step-4 See Diff (Tacked VS Staged)
Do some changes in any file, In my case, I want to do some chnge in the file NewFile.txt.
  
-Now, Open File "NewFile.txt" in any TextEditor.
  
- I'm writing "This file content has been changed!!. " and save the file.
  
``` git diff ``` & hit the enter
  
output
``` 
  
diff --git a/NoteFile.txt b/NoteFile.txt
index 6c229d8..f88df25 100644
--- a/NoteFile.txt
+++ b/NoteFile.txt
@@ -136,9 +136,9 @@ dUSHYANTsINGH

-My First Name is Dushyant


+My Full Name is Dushyant Singh

```
  ``` --- a/NoteFile.txt ``` means something has been deleted in the file
 ``` +++ b/NoteFile.txt ``` means something has been added in the file
  
 ``` -My First Name is Dushyant ```  Minus(-) sign denote delete, so this line has been deleted in the file First
 ``` +My Full Name is Dushyant Singh  ``` plus(+) sign denote delete, so this line has been added in the file First
 
 This diffracnes between Tracked and Staged file,
  
  
## Step-4 See Diff (Staged VS Commited)
  
``` git diff --staged ``` & hit the enter
  
output
``` 

```
  Null output means there is no diffrance between staged and commited file.
 
## Step-5 commit the earlier change
``` git add . ``` or your can give your perticulae file name ``` git add NewFile.txt ``` & hti the enter

See the diffrance before commiting
``` git diff --staged ``` & hit the enter

  output
  ```
  diff --git a/NoteFile.txt b/NoteFile.txt
index f88df25..f464f91 100644
--- a/NoteFile.txt
+++ b/NoteFile.txt
@@ -138,7 +138,7 @@ dUSHYANTsINGH


-My First Name is Dushyant
+My Full Name is Dushyant Singh

```
  
``` --- a/NoteFile.txt ``` means something has been deleted in the file
  
 ``` +++ b/NoteFile.txt ``` means something has been added in the file
  
 ``` -My First Name is Dushyant ```  Minus(-) sign denote delete, so this line has been deleted in the file First
  
 ``` +My Full Name is Dushyant Singh ``` plus(+) sign denote delete, so this line has been added in the file First
 
  
  
  ``` git commit -m "Second commit" ``` & hit the enter  

  output
  
  ```
 [master decdf92] Second commit
 1 file changed, 1 insertion(+), 1 deletion(-)
```
  xxxxxxxxxx END OF PRACTICE XXXXXXXXX
  
</details>


## Git -am "Your Commit": commit without staging

Unstages file, keeping the file changes
  
<details>
 Lev.1 <summary>Click to expand! </summary>
 
``` Git -a -m "commit message??? ``` OR ``` Git -am "commit message" //Unstages file, keeping the file changes
  
Note: This command only used for already tracked file not for new untracked file. Once you need to track the file.
</details>

### @Practice Time 


<details>
  <summary>Click to expand!</summary>
 
How to implement commit changes with without stagging in our project.

### Step-1.0 initialization

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
        .gitignore
        ExcleFile.xlsx
        NoteFile.txt
        WordFile.docx
        new%file.txt

nothing added to commit but untracked files present (use "git add" to track)
 ```
 
 ## Step-1.1 Add file from Working Dir to Stagging Area.

- type ``` git add . ``` & hit the enter // if you want to add all file or spacific you can use ``` . ``` Or ``` --a ``` OR ``` NoteFile.txt ```

- type ``` git status ``` & hit the enter 

output

``` 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:  .gitignore
        new file:   ExcleFile.xlsx
        new file:   NoteFile.txt
        new file:   WordFile.docx
        new file:   new%file.txt

```
Color Diffrance Red to Green (Red means Your file is tracking not in Stagging area. or Unmodify & Green Means you file is add into Stagging area with Modiifide)

### Step-1.2 Commit your file

- type ``` git commit -m "First Commit" ``` & hit the enter 

- output

```
[master (root-commit) 9c6946c] first Commit
 4 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 .gitignore
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

Do some changes in any file, In my case, I want to do some chnge in the file NewFile.txt.
  
-Now, Open File "NewFile.txt" in any TextEditor.
  
- I'm writing "This is Dushyant Singh." and save the file.
  

## Step-2 Use git -am "commit message" cmd
- type ``` git -am "Second Commit ``` & hit the enter 

- output

```
[master b9241af] Second Commit
 1 file changed, 2 insertions(+), 1 deletion(-)

```
- type ``` git status ``` & hit the enter 

- output 

``` 
On branch master
nothing to commit, working tree clean

```

XXXXXXXXX End of Praticle  XXXXXXXXX
</details>
  
 
## Git mv OldFileName.txt NewFileName.txt: Renaming the file

<details>
<summary>Click to expand! </summary>
 
``` git mv [existing-path] [new-path] ```
// change an existing file path and stage the move

</details>
  
## Git rm new_file.txt: Remove the file
<details>
<summary>Click to expand! </summary>
 
``` git rm [existing-path]  ```
// delete the file/dir
</details>

 
## Git rm --cached new_file.txt: Remove the file
<details>
<summary>Click to expand! </summary>
 
``` git rm --cached [existing-path]  ```
// untrack file after file added in .gitignore. the file has commited many time. this command is used to untrack the file from the git system.
</details>
  </details>
  
  ## Git log --amend: merge the pervious commits with your new commit
<details>
<summary>Click to expand! </summary>
 
``` git log --amend  ```
// used to do the merge in pervious commit with your new commit
</details>
  </details>
