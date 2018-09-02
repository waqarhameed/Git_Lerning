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
>
>
To clone existing repo
      > git clone repo-url folder-path    


To create repo in folder-path
      > git init folder-path	
>
>
## 2. Git Basic commands

<a name="removing-local-files"></a>

### 2.1 Removing local files

To Dry run, what will be deleted
	> git clean -n -d or (-nd)	
To interactive deletion
	> git clean -i
To remove directories
    >git clean -f -d or (-fd)
To remove directories from submodules
    >git clean -f -f -d or (-ffd)
    
To remove ignored files
	> git clean -f -X or (-fX)
	
To remove ignored and non-ignored files
	> git clean -f -x or (-fx)
	





