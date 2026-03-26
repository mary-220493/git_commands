## STEP -2

## 1.GIT CONFIGURATION COMMANDS

## 1.git config --user.name

Command name:
git config --user.name


Syntax:
git config --user.name "mary-220493"


Purpose:
sets your git username globally.

Example:
git config --global user.name "mary"

## 2.git config --user.email

Command name:
git config --user.email


Syntax:
git config --user.email "n220493@rguktn.ac.in"

Purpose:
Sets your git email globally.

Example:
git config --user.email "marysripadam@gmail.com"


## 3. git config --list

Command name:
git config --list

Syntax:
git config --list

Purpose:
Displays all Git configuration settings.

## 4. git config --unset user.name
Command name:
git config --unset 


Syntax:
git config --unset user.name "mary-220493"

Purpose:
Removes a specific configuration name.

## 5.git config --unset user.email
Command:
fit config --unset user.email




screenshot proof:
![unset screenshot](screenshots/unset.png)



Syntax:
fit config --unset user.email "n220493@rguktn.ac.in"

Purpose:
Removes a specific configuration email..

## git config --global user.name "madhu-220493"
## git config --global user.email "n220493@rguktn.ac.in"

screenshot proof:
![username screenshot](screenshots/username.png)


## 2.  REPOSITORY SETUP COMMANDS

## 1.git init
syntax:
git init

Purpose:
Creates a new empty git repository in the current folder.

Example:
git init

## 2. git clone
syntax:
git clone <repository-url>

Purpose:
Copies an existing remote repository to your local system.

Example:
git clone https://github.com/user/project.git

## 3. git clone --branch
syntax:
git clone --branch <branch-name>
<repository-url>

Purpose:
Clones a specific branch of a repository instead of the default branch.

Example:
git clone --branch develop
https://github.com/user/project.git

## 4. git clone --depth
syntax:
git clone --depth <number><repository-url>

Purpose:
Creates a shallow clone with limited commit history to save time and space.

Example:
git clone --depth 1
https://github.com/user/project.git


## 3.REPOSITORY STATUS & INSPECTION

## 1. git status
syntax:
git status

purpose:

Shows the current status of your repository.
It tells:

Which files are modified

Which files are staged

Which files are untracked

example:
git status

screenshot proof:
![user screenshot](screenshots/git_status.png)

## 2.GIT LOG

SYNTAX:
GIT LOG

purpose:
displays complete commit history of the repository.
It shows:
commit id
author name
date
commit message


Example:
git log

screenshot proof:
![user screenshot](screenshots/git_log.png)


## 3.GIT LOG --ONELINE


Syntax:
git log --oneline

purpose:
shows commit history in short form(one line per commit)

Example:
fit log --oneline



