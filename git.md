# install
https://git-scm.com/download/win

# config
```
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"
```
# create repository
## create dir
```
$ mkdir learngit
$ cd learngit
$ pwd
```
## init repository
```
$ git init
```

# manage files
## create file
```
$ touch readme.txt
$ vi readme.txt
```
```
Git is a version control system.
Git is free software.
```
## add file to repository
```
$ git add readme.txt
$ git commit -m "wrote a readme file"
```
## modify file
```
vi readme.txt
```
## inquire repository status
$ git status
## see detailed modify
$ git diff readme.txt
## submit again
$ git add readme.txt
$ git status
$ git commit -m "add distributed"
$ git status
## show changes
$ git log

# version
## show version
- head^
- head^^
- head^^^
- head\~100

## version back
```
$ git log
$ git log --pretty=oneline
$ git reset --hard HEAD^
$ git reflog
$ git reset --hard [commit id]
```
> revert A → B → C to A → B → C → B
## stage magage
$ git diff HEAD -- readme.txt
## revocate
### after git add
$ git checkout -- readme.txt
$ git restore --stage readme.txt
### before git add
$ git restore readme.txt
$ git reset HEAD <file>
## delete file
$ rm file.txt
$ git rm file.txt
$ git commit -m ""

# remote repository
$ git config --golbal http.proxy http://127.0.0.1:1080
## push
$ git remote add origin git@github.com:DavidJinThree/learngit.git
$ git push -u origin master
## clone
$ git config http.sslVersion t1sv1.2
$ git clone https://github.com/DavidJinThree/starsCollector

# branch manage
## create and merge
$ git branch dev
$ git switch -c dev
$ git switch master
$ git branch
$ git merge dev
$ git branch -d dev

## fix conflicts
$ git switch -c featurel
$ git add readme.txt
$ git commit -m "AND simple"

$ git switch master
$ git add readme.txt
$ git commit -m "& simple"

$ git merge featurel
$ git status
$ vi readme.txt
$ git add readme.txt
$ git commit -m "conflict fixed"
$ git log --graph --pretty=oneline --abbrev-commit

$ git branch -d featurel

## branch manage strategy

## bug branch
$ git stash

# tag management
## create tag
$ git tag <tagname>
$ git tag -a <tagname> -m "xxx" <commit id>
$ git tag
$ git show <tagname>
## delete tag
$ git tag -d v0.1
### push tag
$ git push origin v1.0
$ git push prigin --tags
### delete remote tag
$ git tag -d v0.9
$ git push origin :refs/tags/v0.9
