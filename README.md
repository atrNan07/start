# start
following apna-college tutorial
<br><br>
**1. CONFIG** <br>
```python
git config --global user.name "<username>"
git config --global user.email "<email address>"
git config # to check all
```

**2. clone n status**<br>
```python
git clone <git link>   # to clone git repository into local (laptop/ pc)
git status   # to check status of git tracking
```
some others : <br>
```python
a. cd <file name>   # to change directory (file)
b. ls    # shows files that can be seen 
c. ls -a    # shows all files, the hidden files also, here .git means git is tracking that file
```

**3.add n commit**<br>
two step process - first add then commit<br>
```python
git add <file name>   # to prepare the file to get committed
git add .  # to add all changes
```
```python
git commit -m "some message"
```

**4.push**<br>
to push back into original repository
```python
git push origin main # origin: cloned repository name, main: branch
```

**5. ADDING NEW REPO FROM LOCAL**<br>
pushing local file to remote (git)<br>
```python
cd .. # to esc the current directory
```
```python
git init # to initialise git tracking in that directory
git remote add origin <link> # to get the repo where 'push' will be done, 'origin' : name
git branch # which branch, 'main'/ 'master' by default
git branch -M <new name> # to rename branch
git push origin main
```

**6. BRANCHES**<br>
they exist so that different specialised teams can work on a copy of the main code and then merge all the different branches together<br>
```python
git branch   # check branch
git branch -M <new name>   # rename branch
git checkout <branch name>   # to switch branch
git checkout -b <new branch name>   # create new branch
git branch -d <branch name>   # delete branch
git push -u origin main # next time 'git push' automatically adds origin main
```
changes in one branch wont be shown in the other branch.<br>
```python
git push origin <branch name> # to push in that branch only
```
**merging branches**<br>
```python
git diff <branch name>  # to check the differences in the 2 branches
git merge <branch name> # to merge the branches
```
PULL REQUEST is another way used in companies mainly to merge<br>
when MERGE CONFLICT arise ie git cant itself decide which to keep and which not, we do it ourselves, other git can do it on its own.<br>

**7. UNDOING CHANGES**<br>
```python
git reset <file name>  # goes back to no 'adds' initial code
git reset # resets all files to before 'add'

git reset HEAD~1  # 'HEAD' is the latest commit, makes latest -1 the new 'HEAD'

git reset <commit hash>.  # goes back to that commit but still keps the changes
git reset --hard <commit hash>  # removes the changes after entirely

git log  # to check commit log
```

**8. FORK**<br>
to get rough copy of other repository on your profile<br>