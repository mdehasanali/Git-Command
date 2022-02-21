<!-- Readme MarkDown Create for Git and Github -->

# আসসালামু আলাইকুম ওয়া রাহমাতুল্লাহি ওয়াবারকাতুহু

1. git?
   - git is a version control software
   - It keep track of code changes
   - It helps to collaborate in a project
   - It is installed and maintained locally
   - It provides Command Line Interface (CLI)
   - Released in April 7, 2005
   - Developed by Linus Torvalds & Junio C Hamano
2. github?
   - GitHub is a hosting service where we can keep our git repositiory/folders
   - It is maintained on cloud/web
   - It provides Graphical User Interface (GUI)
   - Founded in 2008


## Git Downoad

- Download and install git on your pc: https://git-scm.com/
- check git version: open terminal or cmd then use the command `git --version` to find out whether git is installed or not. if git is installed it will return a version number of git.

<p>Git File Download then install</p>

## Github Account Create

- sign in to your github account (https://www.github.com)
- create a git repository

## Git Config Commands

1.  check all configuartion options: `git config`
2.  set global user name and user email for all repository/git folders (if you want to set different username and email for different git repository then remove --global)
    - set global user name: `git config --global user.name "Md. Ehasan Ali"`
    - set global user email: `git config --global user.email "mdehasanali100@gmail.com"`
3.  list all git configuration:
    - list all the configuration: `git config --list`
    - list user name: `git config user.name`
    - list user email: `git config user.email`
4.  change global username & email
    - change global user name: `git config --global user.name "PUT_NEW_USER_NAME_HERE"`
    - change global user email: `git config --global user.email "PUT_NEW_USER_EMAIL_HERE"`

```git

git config --global user.name "Name"
git config --global user.email "explane@gmail.com"

```

# Git file Initialize Commands

git file Initialize korar jonno ati use kora hoi

```

git init

```

# Git file Initialize remove Commands

git file Initialize remove

```

rm -rf .git


```

# Git file staging Commands

1.  adding files to stagging area:

- `git add fileName` add a file in staging area / index
- `git add .` add all files of directory to stagging area not subdirectory
- `git add -A` add all files of directory and subdirectory to stagging area
- `git rm --cached fileName` unstage a file from staging area
- `git diff` - checking the differences of a staged file
- `git restore fileName` - restore the file

```

git add <file name>
git add --all
git add -A
git add .

```

# Git Update Status Commands

update check for git

```

git status

```

# Git message Commands

- `git commit -m "message"` move the file to local repository from stagging area

```

git commit
git commit -m "Your Message"

```

# Git file add or Git message Commands

```

git commit -am "Your Message"
git add -A && git commit -m "Your Message"

```

# Git reset Commands

- `git reset --soft HEAD^` uncommit the commit in HEAD and move to staging area
- `git reset HEAD^` uncommit the commit in HEAD and move to unstaging / working area
- `git reset --hard HEAD^` uncommit the commit in HEAD and delete the commit completely with all the changes

```

git reset
git reset soft HEAD~
git reset HEAD~
git reset --hard HEAD~

```

# Git revert HEAD Commands

```

git revert (commit-id)
git revert HEAD (commit-id)

```

# Git All Ditails Show Commands

- `git log` check the commit history

```

git log
git log --oneline

```

# Git Clone Commands

```

git clone URL
git clone URL foder_name

```

# Git Remote Commands

- check remote connection: `git remote` or `git remote -v`
- `git remote add name <REMOTE_URL>` example: git remote add origin http://...

```

git remote add origin http://...

```

# Git Push Commands

- push a branch `git push -u origin branch_name`
- push all branches `git push --all`
- pull from a repo: `git pull` which is equivalent to git fetch + git merge

```

git push -u origin master
git push origin master -f
git push

git pull

git fetch

```

# Git restore Commands

```

git restore <file name>

```

```

git show <Serial Number>
git checkout <Serial Number>

```

# Git Branch Commands

- Branch is a new and separate branch of master/main repository
- create a branch `git branch branch_name`
- List branches `git branch`
- List all remote branches `git branch -r`
- List all local & remote branches `git branch -a`
- move to a branch `git checkout branch_name`
- create and move to a branch `git checkout -b branch_name`
- delete a branch: `git branch -d branch_name`
- merge branches:
  ```
    git checkout branchName
    git merge branchName
  ```
- `git log --oneline --all --graph`

```

git branch

git branch <branch_name>
git checkout <branch_name>

git checkout -b <branch_name>

git merge <branch_name>

```

# Git git Ignore Commands

- create a .gitignore file and add the things you do not want to add in the stagging area
- Inside .gitignore we can keep secret files, hidden files, temporary files, log files
- `secret.txt` secret.txt will be ignored
- `*.txt` ignore all files with .txt extension
- `!main.txt` ignore all files with .txt extension without .main.txt
- `test?.txt` ignore all files like test1.txt test2.txt
- `temp/` all the files in temp folders will be ignored

```
.gitignore
```
