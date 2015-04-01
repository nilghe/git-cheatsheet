# Git Cheatsheet

Simple collection of explainations, tips, and snippets for git that I had troubles with. 

## rebase

[How to do a damned git rebase](http://stackoverflow.com/a/9147389/1052068)

## revert your uncommited changes

Sometimes, you just mess things up and you need to start over. As long as you have not commited anything then you can simple reset to the HEAD (go back to the last commit on your machine). Just be aware you will lose everything that was not tracked. But sometimes you just want to forget what you have done.

`git reset --HARD`
