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

Patricks-MacBook-Pro:test pb$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   css/main.css
        new file:   css/reset.css
        new file:   index.html
        new file:   js/main.js

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        git-instructions.md

Patricks-MacBook-Pro:test pb$ git addgit-instructions.md
git: 'addgit-instructions.md' is not a git command. See 'git --help'.
Patricks-MacBook-Pro:test pb$ git add git-instructions.md
Patricks-MacBook-Pro:test pb$ git status 
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   css/main.css
        new file:   css/reset.css
        new file:   git-instructions.md
        new file:   index.html
        new file:   js/main.js

Patricks-MacBook-Pro:test pb$ git rm --cached reset.css
fatal: pathspec 'reset.css' did not match any files
Patricks-MacBook-Pro:test pb$ git rm --cached css/reset.css
rm 'css/reset.css'
Patricks-MacBook-Pro:test pb$ git commit -m "We have made files..That's it"
[master (root-commit) 7566c1f] We have made files..That's it
 4 files changed, 75 insertions(+)
 create mode 100644 css/main.css
 create mode 100644 git-instructions.md
 create mode 100644 index.html
 create mode 100644 js/main.js
Patricks-MacBook-Pro:test pb$ 