# git_scenario

- [git-scenario](http://gogojimmy.net/2012/02/29/git-scenario/)

- [source](https://sdwh.dev/posts/2020/05/Git-100/#%E6%83%85%E5%A2%83-%E6%AA%A2%E8%A6%96-Commit-%E7%B4%80%E9%8C%84-%E6%90%9C%E5%B0%8B%E9%97%9C%E9%8D%B5%E5%AD%97)

- [rebase](https://ithelp.ithome.com.tw/articles/10277786)

- [practice-git](https://github.com/grayghostvisuals/practice-git)

### Git Commands
#### Start a working area

```
git clone <repo> //Clone a repository into a new directory
git init         //Create an empty Git repository or reinitialize an existing one
```

#### Set up identifiy

```
git config --global user.name "UserName"
git config --global user.email username@example.com
```

#### Work on the current change

```
git add <file>              //add file
git rm <file>               //remove file
git mv <file> <folder_path> //move file to new folder
```

#### Commit

```
git commit -m "commit msg"
git commit -am "commit msg"        //commit all changed file
git commit --amend -m "commit msg" //fix last commit
git reset HEAD^ --soft             //reset to last commit but remain changes
git reset HEAD^ --hard             //reset to last commit but delete changes
git tag "tag_name"                 //add tag to a commit
git reflog                         //track git change log SHA
git reset <SHA> --hard             //reset to that status
```

#### Check history and state

```
git log     //show log exit press 'q'
git status  //show current status.
git show    //show various types of objects
git bisect  //use binary search to find the commit that introduced a bug
git diff    //show changes between commits, commit and working tree, etc
git grep    //print lines matching a pattern
```

#### Branch

```
git branch                            //show local branch
git branch -r                         //show remote branch
git branch -a                         //show all branch
git branch <branch_name>              //create branch
git branch -d <branch_name>           //delete local branch
git branch -r -d <remote_branch_name> //delete remote branch
git push --set-upstream origin master //push a branch that not exit in remote.
git checkout -b "branch_name"         //create branch and checkout to that branch
git checkout <branch_name>            //switch branch
```

#### Stash

```
git stash       //stash current change
git stash apply //retrieve last stash
git stash pop   //pop last stash and remove from stash
git stach list  //show all stash list
git stach clear //clear all stash
```

#### Merge

```
git merge <branch_name>             //merge branch into current branch
git merge <branch_name> --no-commit //merge branch into current branch without commit
git cherry-pick <SHA>               //merge specific commit into current branch
git rebase                          //reapply commits on top of another base tip
```

#### Collaborate

```
git fetch       //download objects and refs from another repository
git pull        //fetch from and integrate with another repository or a local branch
git push        //update remote refs along with associated objects
```
