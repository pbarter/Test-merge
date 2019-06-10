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
Patricks-MacBook-Pro:test pb$ git commit "added commit log"
error: pathspec 'added commit log' did not match any file(s) known to git
Patricks-MacBook-Pro:test pb$ git commit -m "added commit log"
On branch master
Changes not staged for commit:
        modified:   git-instructions.md

Untracked files:
        css/reset.css

no changes added to commit
Patricks-MacBook-Pro:test pb$ git rm --cached reset.css
fatal: pathspec 'reset.css' did not match any files
Patricks-MacBook-Pro:test pb$ git add --all
Patricks-MacBook-Pro:test pb$ git commit -m "added commit log"
[master 1f96a4a] added commit log
 2 files changed, 185 insertions(+), 1 deletion(-)
 create mode 100644 css/reset.css
Patricks-MacBook-Pro:test pb$ git log
commit 1f96a4a04f046140f45d7e6cd03e3de2d955a4a2 (HEAD -> master)
Author: Patrick B <patrick.barter@rogers.com>
Date:   Mon Jun 10 11:48:50 2019 -0400

    added commit log

commit 7566c1fba0af1bb46d1701fb89fe3fe2b805db7c
Author: Patrick B <patrick.barter@rogers.com>
Date:   Mon Jun 10 11:46:02 2019 -0400

    We have made files..That's it
Patricks-MacBook-Pro:test pb$ git help
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout    Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
Patricks-MacBook-Pro:test pb$ git status
On branch master
nothing to commit, working tree clean
Patricks-MacBook-Pro:test pb$ git remote add origin https://github.com/pbarter/Test-merge.git
Patricks-MacBook-Pro:test pb$ git push -u origin master
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (12/12), 3.63 KiB | 1.82 MiB/s, done.
Total 12 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/pbarter/Test-merge.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.
Patricks-MacBook-Pro:test pb$ 