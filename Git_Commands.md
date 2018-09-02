## 1. Git Environment Setup

### 1.1 First time git setup

* Install git client from [here](https://git-scm.com/downloads) and optionally GUI Client from [here](https://git-scm.com/downloads/guis)  
Then verify your installation:	
> git --version
	
* Setup Your Identity  
Setup your name and email
	
> git config --global user.name "Alpha Bravo"
> git config --global user.email "alpha.bravo.gmail.com"
	
* To colorize output of git in terminal

> git config --global color.ui auto
	

### 1.2 Setup Alias

* git status + git st

> git config --global alias.st status
	
* git log -n 3 --oneline = git logs
> git config --global alias.logs 'log -n 3 --oneline'

	
### 1.3 Verify Settings

> git config --global -list

## 2 Git repos

### 2.1 Creating repo


 To clone existing repo
    > git clone repo-url folder-path    
 To create repo in folder-path
    > git init folder-path	


## 2. Git Basic commands

  <a name="removing-local-files"></a>

### 2.1 Removing local files

To Dry run, what will be deleted
> git clean -n -d or (-nd)

To interactive deletion
    > git clean -i
To remove directories
    > git clean -f -d or (-fd)
To remove directories from submodules
    > git clean -f -f -d or (-ffd)
    
To remove ignored files
> git clean -f -X or (-fX)
	
To remove ignored and non-ignored files
> git clean -f -x or (-fx)
### 2.2 Staging/UnStaging files
	
To stage all files in index 
   > git add .
To stage particular file in index
   > git add some-file.txt
Add -f flag, if files are ignored by .gitignore
    > git add -f some-ignored-file.txt
	
To unstage files from index
    > git reset
    > git reset HAED -- some-file.txt
	
To reset changed files and (remove new files if staged)
> git reset --hard
	
To remove unwanted file from git index (but keep file on disk)
> git rm --cached some-file.txt
    > git rm -r --cached some-directory/
	
Discard changes in the working directory
> git checkout -- file.txt
   > git checkout -- .
	
### 2.3 Git Diff	
	
To see what you�ve changed but not yet staged
> git diff
	
To see what you�ve changed but not yet staged
> git diff --staged
	
### 2.4 Committing Your Changes

To commit your staged changes
> git commit -m "Well written commit message"	
	
To skip staging files step use -a
> git commit -a -m "I committed without staging these files"
	
To change commit message of last commit
> git commit --amend
	
To change commit author info
> git commit --amend --author="Alpha Bravo <alpha.bravo@gmail.com>"
		
### 2.5 Viewing Your Changes

To view last 3 commits
>> git log -n 3
	
To view commits with differences (--patch)
> git log -p -n 3
	
## 3. Working with branches

<a name="git branches"></a>

### 3.1 Creating/Deleting branches

To list all branches
   > git branch  (-a for remote branches)
	
To create branch named br-1
   > git branch br-1
	
To create branch named br-2 and checkout
   > git branch br-2
	
To switch branch
   > git checkout branch2
	
To delete branch
   > git branch -d branch-name (-D to forcefully delete)
	
To delete remote branch
  > git push origin :branch-name	



	


