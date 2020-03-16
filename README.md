# Custom commands for git

## How to use
1. Put the command bash files in a folder
2. Add the folder path to your **PATH** variable in your bash config file (**.bashrc** in Linux)
  * Example: `export PATH="$PATH:$HOME/Work/custom-git-commands"`
3. Source the bash config file
* `source ~/.bash_profile`
4. Set execution privileges to the command bash files
5. That's it.

<br/>

## Commands
### 1. git get-changes \<remote-branch>
Scenario:

* Suppose you are working on a *local* branch named `kaaj-kortesi`
* Somebody added their changes to a *remote* branch `agaye-ache`
* You need those changes on your local branch. 
* So you `stash-> switch branches -> pull from remote -> switch branches -> rebase -> apply stash`
* Why the hustle?


**To get the updates from `agaye-ache`, just use:**
```
git get-changes agaye-ache
```

<br/>

### 2. git acp \<commit-message> (Add-Commit-Push)
Scenario:

* You added a quickfix.
* You just want to add all changes and push.
* Why go through the steps of `add -> commit -> push`?

**To just stage and push everything, right here right now, just use:**
```
git acp "A bad commit message"
```

<br/>

### 2. git dch (Delete Commit History)
Scenario:

* You want a fresh start with all your previous codes intact.
* You'd need to `create a temp ORPHAN branch -> add all and commit to that branch -> delete old branch -> rename temp to the old branch name -> force push changes to remote`

**Instead of those steps, just use:**
```
git dch
```
