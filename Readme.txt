
maristuser@HC0005-29 MINGW64 ~
$ git-version
bash: git-version: command not found

maristuser@HC0005-29 MINGW64 ~
$ git - version
Unknown option: -
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

maristuser@HC0005-29 MINGW64 ~
$ git -version
Unknown option: -version
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

maristuser@HC0005-29 MINGW64 ~
$ git--version
bash: git--version: command not found

maristuser@HC0005-29 MINGW64 ~
$ git --version
git version 2.9.2.windows.1

maristuser@HC0005-29 MINGW64 ~
$ git config --global user.name "Manfred Cabintoy"

maristuser@HC0005-29 MINGW64 ~
$ git config --global user.email "manfred.cabintoy1@marist.edu"

maristuser@HC0005-29 MINGW64 ~
$ git config --global color.ui "auto"

maristuser@HC0005-29 MINGW64 ~
$ git config --global core.editor "nano"

maristuser@HC0005-29 MINGW64 ~
$ cd the-address-of-the-Desktop
bash: cd: the-address-of-the-Desktop: No such file or directory

maristuser@HC0005-29 MINGW64 ~
$ cd C://Users/maristuser/Desktop

maristuser@HC0005-29 MINGW64 ~/Desktop
$ pwd
/c/Users/maristuser/Desktop

maristuser@HC0005-29 MINGW64 ~/Desktop
$ mkdir toasty

maristuser@HC0005-29 MINGW64 ~/Desktop
$ cd toasty

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty
$ git init
Initialized empty Git repository in C:/Users/maristuser/Desktop/toasty/.git/

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ touch Readme.txt

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git status
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        Readme.txt

nothing added to commit but untracked files present (use "git add" to track)

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git add Readme.txt

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git status
On branch master

Initial commit

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   Readme.txt


maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git commit -m "Add Readme.txt"
[master (root-commit) cc910c0] Add Readme.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Readme.txt

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ touch test.txt

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git add test.txt

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git commit -m "test.txt"
[master 8d6051a] test.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test.txt

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git remote add origin https://github.com/toasty1989/toasty.git

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git remote -v
origin  https://github.com/toasty1989/toasty.git (fetch)
origin  https://github.com/toasty1989/toasty.git (push)

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master


maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push origin master
Fatal: AggregateException encountered.
Username for 'https://github.com': git push origin master
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/toasty1989/toasty.git/'

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push origin master
Fatal: AggregateException encountered.
Username for 'https://github.com':
remote: Anonymous access to toasty1989/toasty.git denied.
fatal: Authentication failed for 'https://github.com/toasty1989/toasty.git/'

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push origin master
Fatal: AggregateException encountered.
Username for 'https://github.com':
remote: Anonymous access to toasty1989/toasty.git denied.
fatal: Authentication failed for 'https://github.com/toasty1989/toasty.git/'

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push test.txt
fatal: Invalid gitfile format: test.txt
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push "test.txt"
fatal: Invalid gitfile format: test.txt
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git remote -v
origin  https://github.com/toasty1989/toasty.git (fetch)
origin  https://github.com/toasty1989/toasty.git (push)

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master


maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push -u origin master
Fatal: AggregateException encountered.
Username for 'https://github.com': git push -u origin master
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/libexec/git-core/git-gui--askpass'
Password for 'https://git push -u origin master@github.com':
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/toasty1989/toasty.git/'

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git -u origin master
Unknown option: -u
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push -u origin master
Fatal: AggregateException encountered.
Username for 'https://github.com':
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/libexec/git-core/git-gui--askpass'
Password for 'https://github.com':
remote: Anonymous access to toasty1989/toasty.git denied.
fatal: Authentication failed for 'https://github.com/toasty1989/toasty.git/'

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
$ git push origin master
Fatal: AggregateException encountered.
Username for 'https://github.com': toasty1989
Counting objects: 5, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 439 bytes | 0 bytes/s, done.
Total 5 (delta 0), reused 0 (delta 0)
To https://github.com/toasty1989/toasty.git
 * [new branch]      master -> master

maristuser@HC0005-29 MINGW64 ~/Desktop/toasty (master)
