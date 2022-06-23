# git_scenario

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
```

#### Check history and state

```
git log     //show log exit press 'q'
git status  //show current status.
git show    //show various types of objects
git bisect  //Use binary search to find the commit that introduced a bug
git diff    //Show changes between commits, commit and working tree, etc
git grep    //Print lines matching a pattern
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