### **Git Commands**

##### **1. git config**

**Definition**:

Used to set and view Git configuration details like username and email.

**Command:**

git config --list

**Output:**

user.name=Jyothi Prasanna

user.email="---email---"

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **2. git init**

**Definition:**

Creates a new Git repository in the current folder.

**Command:**

git init

**Output:** Initialized empty Git repository in C:/Users/GVPW/Desktop/devops/.git/

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### 3\. git status

**Definition**:

Shows the current state of the working directory, including modified, staged, and untracked files.

**Command:**

git status

**Output:**

On branch master

No commits yet

Changes to be committed:

&#x20; new file: hi.txt

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **4. git add**

**Definition:**

Moves files from the working directory to the staging area so they can be committed.

**Command:**

git add hi.txt

**Output:**(no output means the command was successful)

Check with:

git status

**Output:**

Changes to be committed:

&#x20; new file: hi.txt

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **5. git commit**

**Definition:**

Saves staged changes permanently in Git history with a message.

**Command:**

git commit -m "Add hi.txt"

**Output:**

\[master (root-commit) abc1234] Add hi.txt

&#x20;1 file changed, 1 insertion(+)

&#x20;create mode 100644 hi.txt

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **6. git branch**

**Definition:**

Creates and manages different versions (branches) of a project.

**Command:**

git branch feature

**Output:**(no output means success)

git branch

**Output:**

\* master

&#x20; feature

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **7. git checkout**

**Definition:**

Used to switch between branches.

**Command:**

git checkout feature

**Output:**

Switched to branch 'feature'

git branch

**Output:**

&#x20; master

\* feature

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **8. git merge**

**Definition:**

Combines changes from one branch into another branch.

**Command:**

git checkout master

git merge feature

**Output:**

Updating abc1234..def5678

Fast-forward

&#x20;hi.txt | 1 +

&#x20;1 file changed, 1 insertion(+)

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **9. git remote**

**Definition:**

Connects your local Git repository with a remote repository like GitHub.

**Command:**

git remote add origin https://github.com/username/DEVOPS.git

**Output:**(no output means success)

git remote -v

**Output:**

origin  https://github.com/username/DEVOPS.git (fetch)

origin  https://github.com/username/DEVOPS.git (push)

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **10. git clone**

**Definition:**

Creates a local copy of an existing remote Git repository.

**Command:**

git clone https://github.com/username/DEVOPS.git

**Output:**

Cloning into 'DEVOPS'...

Receiving objects: 100% (5/5), done.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **11. git push**

**Definition:**

Uploads local commits to a remote repository.

**Command:**

git push origin master

**output:**

Enumerating objects: 5, done.

Writing objects: 100% (5/5), done.

To github.com:username/DEVOPS.git

&#x20;  abc1234..def5678  master -> master

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### **12. git pull**

**Definition:**

Downloads changes from a remote repository and merges them into your local branch.

**Command:**

git pull origin master

\-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

##### Git Workflow

git config

&#x20;     ↓

git init

&#x20;     ↓

git status

&#x20;     ↓

git add

&#x20;     ↓

git commit

&#x20;     ↓

git branch

&#x20;     ↓

git checkout

&#x20;     ↓

git merge

&#x20;     ↓

git remote

&#x20;     ↓

git clone

