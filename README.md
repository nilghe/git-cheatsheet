# Git Cheatsheet

Simple collection of explainations, tips, and snippets for git that I had troubles with. 

## rebase

[How to do a damned git rebase](http://stackoverflow.com/a/9147389/1052068)

## revert your uncommited changes

Sometimes, you just mess things up and you need to start over. As long as you have not commited anything then you can simple reset to the HEAD (go back to the last commit on your machine). Just be aware you will lose everything that was not tracked. But sometimes you just want to forget what you have done.

`git reset --HARD`

## checkout remote branch

I never remember how to do this. I should just make an alias, but where is the fun in that?

* `git fetch`
* `git checkout --track origin/branch_name`

## view git log by author

When you want to see all the commits made by a specific person in your branch. Taken from this [Stackoverflow answer](http://stackoverflow.com/a/4262780/1052068). 

`git log --author="Chris"`
`git log --author=Chris`
`git log --author=Last`

# Delete local and remote branch

You should be keeping your git repo clean, so you want to delete branches locally AND remote. Becareful with this.

`git push origin --delete <branch name> # delete remote branch`
`git branch -d <branch name> # delete local branch only`


# Simple Alias for bash or zsh

Add these so your `~/.zsh` or `~/.bash_profile`

```
alias gits='git status'
alias gita='git add . --all'
alias gitl='git log'
alias gitc='git commit -am'
```


