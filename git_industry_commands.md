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

## 4. GIT LOG --GRAPH
Syntax:
git log --graph

Purpose:
Displays the commit history in a graphical branch structure

Example:
git log --graph

Screenshot proof:
![user screenshot](screenshots/git_log_oneline_graph.png)

## 5.GIT SHOW

Syntax:
git show

Purpose:
shows detailed information about a specific commi,including:
author
date
commit message
code changes

Example:
git show 

Screenshot proof:
![user screenshot](screenshots/git_show.png)

## 6.GIT DIFF
Syntax:
git diff

Purpose:
Shows a difference between modified files and the last commit 

Example:
git diff


## 7. GIT DIFF --STAGED
Syntax:
git diff --staged

Purpose:
Shows the difference between staged files and the last commit.

Example:
git dif --staged


## 8.GIT BLAME

Syntax:
git blame<file-name>

Purpose:
Shows who lst modofied each line in a file.

Example:
git blame<index.html>

Screenshot proof:
![user screenshot](screenshots/git_diff_blame.png)

## 9.GIT REFLOG

Syntax:
git reflog

Purpose:
Shows all actions performed in the repository such as :
Commits
results
checkouts

Example:
git reflog

## 10. GIT SHORTLOG

Syntax:
git shortlog

Purpose:
Shows summary of commits grouped by author.

Example:
git shortlog

Screenshot proof:
![user screenshot](screenshots/git_reflog_shortlog.png)

## 4.FILE TRACKING COMMANDS

## 1.git add
syntax:
git add <file-name>

purpose:
Adds a specific file to the staging area so it will be included in the next commit.

Example:
git add git_industry_commands


## 2.git add .
syntax:
git add .

Purpose:
Adds all modified and new files in the current folder to this sytaging area.

Example:
git add.

## 3.git add -p
syntax:
git add -p

purpose:
Adds changes interactively(part by part) to the staging area.

Example:
git add -p

## 4.git restore
syntax:
git restore <file-name>

Purpose:
restores a file to its last commited version (undoes local changes).

Example:
git restore git_industry_commands

## 5.git restore --staged
Syntax:
git rstore --staged <file-name>

Purpose:
Removes a file from the staging area but keeps the file changes in your working directory.

Example:
git restore --staged <file-name>

Purpose:
Removes a file from the staging area but keeps the files changes in your working directory.

Example:
git restore --staged git_industry_commands

## 6.git rm
Syntax:
git rm <file-name>

Purpose:
Deletes a file from both the working directory and Git repository.

Example:
git rm oldfile.txt

## 7. git mv
Syntax:
git mv <old-file-name><new-file-name>

Purpose:
Used to rename or move a file in Git.
Git tracks the rename automatically.

Example:
git mv file1.txt file2.txt

