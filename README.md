# Custom commands for git

### git get-changes \<remote-branch>
Scenario:

* Suppose you are working on a *local* branch named `kaaj-kortesi`
* Somebody added their changes to a *remote* branch `agaye-ache`
* You need those changes on your local branch. 
* So you `stash-> switch branches-> pull from remote-> switch branches-> rebase-> apply stash`
* Why the hustle?


**To get the updates from `agaye-ache`, just use**
```
git get-changes agaye-ache
