log:

Patricks-MacBook-Pro:test pb$ git init
Initialized empty Git repository in /Users/pb/Desktop/test/.git/
Patricks-MacBook-Pro:test pb$ git status 
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        css/
        index.html
        js/

nothing added to commit but untracked files present (use "git add" to track)
Patricks-MacBook-Pro:test pb$ git ls
git: 'ls' is not a git command. See 'git --help'.

The most similar command is
        log
Patricks-MacBook-Pro:test pb$ ls 
css             img             index.html      js
Patricks-MacBook-Pro:test pb$ git add index.html
Patricks-MacBook-Pro:test pb$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        css/
        js/

Patricks-MacBook-Pro:test pb$ git add css/
Patricks-MacBook-Pro:test pb$ git add js/
Patricks-MacBook-Pro:test pb$ git status 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   css/main.css
        new file:   css/reset.css
        new file:   index.html
        new file:   js/main.js

Patricks-MacBook-Pro:test pb$