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
