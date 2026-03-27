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

## 5.COMMIT COMMANDS

## 1.git commit
Syntax:
git commit

Pupose:
Creates a new commit with the staged files.
when you run this commands,Git opens a text editor to write the commit message.

Example:
git commit

## 2. git commit -m
Syntax:
git commit -m "commit messasge"

Purpose:
Creates a commit with a message directly from the command line without opening an editor.

Example:
git commit -m "Added login page"

## 3. git commit --amend
Syntax:
git commit --amend

Purpose:
Used to modify the most recent commit.
ypu can:
Change the commit message
Add new changes to the last commit

Example:
git commit --amend

Git opens the editor to edit the previous commit message.
Example change:
Added login page and fixed css

## 4. git commit --no-edit
Syntax:
git commit --amend--no-edit

Purpose:
Amends the last commit without changing the commit message.
Useful when you forgot to add a file to the previous commit.

Example:
git add style.css
git commit --amend--no-edit

This:
Adds style.csss
Updates the last commit without editing the message.

## 6.BRANCH MANAGEMENT COMMANDS

## 1. git branch
Syntax:
git branch

Purpose:
Displays the list of branches in the repository.
The current branch  will be marked with *.

Example:
git branch

## 2.git branch -a
Syntax:
git branch -a

Purpose:
Shows all brsnches,including:
Locsl branches
Remote branches

Example;
git branch -a


## 3.git branch -d
Syntax:
git branch -d <branch-name>

Purpose:
Deletes a local branch safely.
Git will not delete the branch if it has unmerged changed.

Exxample:
git branch -d feature-login

This delete the feature-lgin branch.

## 4. git branch -D
Syntax:
git branch -D <branch-name>

Purpose:
Forces deletion of a branch even if it has unmerged changes.

Exmaple:
git branch -D feature-login
This force deletes the branch.

## 5. git checkout
Syntax:
git checkout <branch-name>

Purpose:
Switches from the current branch to another branch.

Example:
git checkout development
This moves from thr current branch to the development branch.

## 6.git checkout -b
Syntax:
git checkout -b feature-login

Purpose:
creates a new branch and switches to it immediately.

Example:
git checkout -b fearure-login

## 7.git switch
Syntax:
git switch <branch-name>

Purpose:
Switches to another branch (modern alternative to checkout).

Example:
git switch main

## 8.git switch -c
synatx:
git switch -c <branch-name>

Purpose:
Creates a new branch and switches to it using the modern command.

Example:
git switch -c new-feature

## 7.MERGE & INTEGRATION COMMANDS

## 1.git merge
syntax:
git merge <branch-name>

Purpose:
Used to combine changes from one branch into another branch.

Example:
git checkout main 
git merge feature-login

## 2. git merge --no-ff
syntax:
git merge --no-ff <branch-name>

Purpose:
Merges a branch but creates a seperate merge commit,evenif a fast-forward merge is possible.

Examples:
git checkout main
git merge --no-ff feature-login


## 8.REMOTE REPOSITORY COMMANDS

## 1. git remote
syntax:
git remote:

Purpose:
Displays the list of remote repositories connected to your local repository.

Example:
gti remote

## 2. git remote -v 
syntax:
git remote -v

Purpose:
Shows remote repository URLs for fetch and push.

Example:
gir remote -v

## 3. gir=t remote add 
syntax:
git remote add <name><repository-url>

Purpose:
Adds a new remote repository to your locsl git project.

Example:
git remote add origin
https://github.com/madhu-220630/myproject.git

## 4.git remote remove
Syntax:
git remote remove <remote-name>

Purpose:
removes a remote repository connection from your project.

Example:
git remote remove origin

## 5. git fetch
Syntax:
git fetch

Purpose:
Downloads new changes from the remote repositories but does not merge them into yoour current branch.

Example:
git fetch origin

## 6.git fetch --all
syntax:
git fetch --all

Purpose:
Fetches changes from all remote repositories.

Example:
git fetch --all

## 7.git pull
syntax:
git pull

Purpose:
Downlloads changes from the remote repositories and merges them automatically into the 
current branch.

Example:
git pull origin main

## 8.git pull --rebase
syntax:
git pull --rebase

Purpopse:
Fetches changes from remote and reapplies your local commits on top pf them,keeping history clear.

Example:
git pull --rebase origin main

## 9.git push
syntax:
git push

Purpose:
Uploads local commits to the remote repository.

Example:
git push origin main

## 10.git push -u origin mbranch-name
syntax:
git push -u origin <branch-name>

Purpose:
Pushes a branch to the remote repository and sets upstream tracking.
After this ,you can simply use git push.

Example:
git push -u origin main

## 11. git push --force
syntax:
git push --force

Purpose:
Forces git to overwrite the remote branch with local changes.

Example:
git push --force origin main


## 9.STASH COMMANDS

## 1.git stash
syntax:
git stash

Purppose:
Temporarily saves your uncommited changes and cleans the working directory so you can 
work something on else.

Example:
git stash

## 2.git stash list
syntax:
git stash list

Purpose:
Displays the list of all saved stashes.

Example:
git stash list

## 3.git stash pop
Syntax:
git stash pop

Purpose:
Apllies the latest stash changes and removes it from the stash list.

Example:
git stash pop

## 4.git stash apply
Syntax:
git stash pop

Purpose:
Apply saved stash changes but keeps the stash in the stash list.

Example:
git stash apply

## 5.git stash drop
Syntax:
git stash drop <stash-id>

Purpose:
Deletes a specific stash entry.

Example:
git stash drop stash@{0}

## 6. git stsash clear
Syntax:
git stash clear

Purpose:
Delete all stash entries permanently.

Example:
git stash clear

## 10.RESET & UNDO COMMANDS

## 1. git reset
syntax:
git reseet <commit-id>

Purpose:
Moves the HEAD pointer to a previous commit.
It is used to undo commits or changes in the repository.

Example:
git reset a34f67b

## 2.git reset --soft
Syntax:
git reset --soft<commit-id>

Purpose:
Moves the HEAD to the specific commit,but keeps all changes staged.
Useful when:
You want to change the last commit message.
combine commits

Example:
git reset --soft HEAD~1

## 3. git reset --mixed
Syntax:
git reset --mixed <commit-id>

Purpose:
Moves HEAD to the specific commit and unstages the changes,but keeps them in the working directory.
This is the deqfault reset mode.

Example:
git reset --mixed HEAD~1

## 4. git reset --hard
syntax:
git reset --hard<commit-id>

Purpose:
Resets:
commit history
staging area
working directory

Example:
git reset --hard HEAD~1

## 5. git revert
Syntax:
git revert
Purpose:
Creates a new commit that reverses the changes of a prevoius commit.
This is safer than reset because it keeps commit history.

Example:
git revert a34f67b

## 6.git clean -f
syntax:
git clean -f

Purpose:
Deletes untracked files from the working directory.

Example:
git clean -f

## 7.git clean -fd
syntax:
git clean -fd

Purpose:
Deletes:
untracked files
untracked directories.

Example:
git clean -fd


## 11. REBASING COMMANDS

## 1. GIT REBASE
syntax:
git rebase <branch-name>

Purpose:
Used to move or reapply commits from one branch onto another branch .
It creates a linear commit history 

Example:
git checkout feaature-login
git rebase main

## 2. git rebase -i
Syntax:
git rebase -i<commit id>        
        or
git rebase -i HEAD ~n

Purpose:
Performs interactive rebasing,allowing you to:
Edit commit message
Combine commits
Reorder commits
remove commits

Example:
git rebase -i HEAD~3

## 3.git rebase --continue
Syntax:
git rebase --continue

Purpose:
Continues the rebasing process after resolving conflicts.
When conflicts happen during rebase:
Fix the conflicting file.
Add them to staging.
Continue rebase.

Example:
git add index.html
git rebase --continue

## 4. git rebase --abort
syntax:
git rebase --abort

Purpose:
Stops the rebase procedd and returns the branch to its original state before rebasing started.

Example:
git rebase --abort

## 12.CHERRY PICK & PATCH COMMANDS

## 1.git cherry-pick
syntax:
git cherry-pick <commit-id>

Purpose:
This command is used to apply a speccific commit from one branch to another branch .
Instead of merging the entire branch,it copies only the selected commit.

Example:
git checkout main
git cherry-pick a1b2c3d

## 2.git format-patch
syntax:
git format-patch <commit-id>    or      git format-patch-n

Purpose:
This command creates patch files (.patch) from commitd.
These patch files can be shared with others or applied to another repository.

Example:
git format-patch-2

## 3. git apply
syntax:
git apply<patch-file>

Purpose:
This command applies changes from a patch file to the working directory.
It does not create a commit automatically.

Example:
git apply 0001-added-login-feature.patch

## 4. git am
syntax:
git am <patch-file>

Purpose:
This commands applies patch files and automatically creates commits.
It is mainly used when patches are recieved through email or shared patch files.

Examplle:
git am 0001-addded-login-feature.patch

## 13.TAGGING COMMANDS

## 1.git tag
syntax:
git tag

Purpose:
Cretaes a tag for the current commit to mark a specific version.

Example:
git tag v1.0

## 2.git tag -a
syntax:
git tag -a <tag-name>-m "message"

Purpose:
Creates an annotated tag with a message for better version information.

Example:
git tag -a v1.1 -m "first stable release"

## 3.git tag -d
syntax:
git tag -d <tag-name>

Purpose:
Deletes an existing local tag.

Exaple:
git tag -d v1.0

## 4. git push origin --tags
syntax:
git push origin --tags

Purpose:
Pushes all local tags to the remote repository.

Example:
git push origin --tags

## 14.SUBMODULE COMMANDS

## 1. git submodule add
syntax:
git submodule add <repository-url>
<folder-name>

Purpose:
Adds another git repository inside the current repository as a submodule.

Example:
git submodule add
https://github.com/user/library.git lib

## 2. git submodule init
syntax:
git submodule init

Purpose:
Initializes the submodule configuration in the local repository.

Example:
git submodule init

## 3. git submodule update
syntax:
git submodule update 

Purpose:
Downloads and updates the submodule content to the correct commit.

Example:
git submodule update

## 15. DEBUGGING COMMANDS

## 1. git bisect
syntax:
git bisect <command>

Purpose:
Helps find the commit that introduced a bug using binary search.

Example:
git bisect start

## 2. git bisect start
syntax:
git bisect start

Purpose:
Starts the bisect debugging process.

Example:
git bisect start

## 3. git bisect good
Syntax:
git bisect good <commit-id>

Purpose:
Marks a commit as working correctly(no bug).

Example:
git bisect good a1b2c3d

## 4. git bisect bad
syntax:
git bisect bad <commit-id>

Purpose:
Marks a commit as containing the bug.

Example:
git bisect bad d5e55f6

## STEP-3

## 1.Create repository

Purpose:
Creates a new project repository on GitHub to store code and files.

Example:
Create a repository named student-management-system on github.

## 2. Add README

Purpose:
Adds a README.md file to describe the project and provide instructions.

Example:
Add a README. explaining the project,features,and how to run the code.

## 3. Add.gitignore

Purpose:
Specifies files or folders that Git should ignore.

Example:
Add.gitignore to ignore files like:
node_modules/
*.log
.env

## 4. Create Issue
Purpose:
Creates a task,bug report,or feature request in the repository.

Example:
Creates an issue titled "Fix login page error".

## 5. Assign issue

Purpose:
Assigns the issue to a team member responsible for fixing it.

Example:
Assign the login bug issue to Madhu.

## 6. Create Branch

Purpose:
Creates a seperate branch to work on new features without affecting the main code.

Example:
Create a branch named login-feature.

## 7. Push Branch

Purpose:
Uploads the local branch to the Github repository.

Example:
git ppush origin login-feature

## 8. Create Pull Request

Purpose:
Request to merge changes from one branch to another(usually to main).

Example:
Create a pull request from login-feature->main

## 9. Review Pull Request

Purpose:
Allows team members to check the code and suggest changes before merging.

Example:
A teammate reviews the pull request and comments on improvements.

## 10. Merge Pull Request

Purpose:
Combines the approved changes into the main branch.

Example:
Merge login-feature branch into main branch.

## 11. Resolve Merge Conflict 

Purpose:
Fixes conflicts when two branches change the same code differently.

Example:
Edit the conflicting file and choose the correct code,then commit.

## 12. Close Issue

Purpose:
Marks the issue as completed after fixing the problem.

Example:
Close the issue "Fix login page error".

## 13. Add Labels

Purpose:
Adds categories to issues or pull requests for better organization.

Example:
Add labels like bug,enhancement,or documentation.

## 14. Add Collaborations

Purpose:
Allows other users to work on the repository.

Example:
Add team members as collaborators so they can push code.
