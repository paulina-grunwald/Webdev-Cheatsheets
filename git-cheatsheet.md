# Git Cheat Sheet

> Written by Paulina Grunwald

> <em>May 2018</em>
<br/>

# 1. About Git
- Created by Linus Torvalds in April 2005.
- Git 1.0 was released at the end of 2005.
- Git is a distributed version control systems.
- Every Git directory on every computer is a full-fledged repository with complete history and full version tracking abilities, independent of network access or a central server.
- Every Git repository is full copy of the repository.

# 2. Useful terminology

__VCS/VCM__ - (version control system/source code manager) tracks changes in your project and allows you to revert files back to the state before certain change has been done. You can revert the entire project to the previous state. It allows you to see previously done changes, who modified the code and when it was done.

__Repository__ - directory that contains all files from your project(as well as certain hidden files). They are used to communicate with Git. t. Repositories
can exist either locally on your computer or as a remote copy on another compute

__Bare repository__ - repository without a working directory. Use bare repository on a remote server to allow multiple contributors to push their work. Think of bare repository as workspace.
down vote. Bare repositories are only changed by transporting changes from other repositories.

__Working directory__ - the area where user can modify the files in the repository before commiting them.

__Commit__ - snapshots of your repository at the time when commit was done. It records metadata for each change made to the repository.

__Remote__ - a link to another git repository.

__File status life cycle__ - movement of the files bewteen stages in the git. Files can be in 4 various stages: ``untracked``, ``tracked``, ``modified``, ``staged``.

__Index__ - describes the repository directory strucure and content at the point in time

__Staging Area__

__SHA__ - ID number for each commit. Each SHA is unique. Every object in Git has its own SHA1.

__Branch__

We have following __git objects__:
- Blobs,
- Trees,
- Commits
- Annotated Tags.



Git has three main states:
- modified,
- staged,
- commited.

``pwd`` -  present working directory<br/>
``mkdir your_folder_name`` -  create new folder
``cd your_folder_name`` - change directory
``rm`` - remove files and directories

Flag is used to alter how a program functions

``-a`` - hidden<br/>
``ls -l`` - shows total numbers of files in the folder
``-l`` - view details of the file<br/>
``-t`` - type<br/>
``-p`` - pretty print<br/>
``ls`` -  print all files in the folder<br/>
``ls -al`` - get all the files including hidden file and their details

``git branch`` - check the list of branches<br/>

## Clone Existing repository
``git clone https://github.com/libgit2/libgit2``

## Create new repo

``git init`` - Initialize empty git<br/> repository in selected folder<br/>
``ls .git`` - check the content of the repo<br/>
``cat .git/config`` - check content of the config file<br/>
``git status`` - check status<br/>
``git config user.name "Joe Doug"`` - add user name<br/>
``git config user.email "name@gmail.com"`` - add e-mail info<br/>

``git add`` - add files to staging area<br/>
``git commit -m "First commit"`` - commit the file with the commit message<br/>
``git log`` - check the list of existing commits<br/>

``git count-objects`` - count objects in the git repo<br/>

``ls -a`` - view all hidden files in the repository

``git show`` - displays information about given commit

``git-cat-file`` - Provide content or type and size information for repository objects

``git tag -a mytag -m "This is my tag" - create a tag

If you want to see what you haven't git added yet:

``
git diff myfile.txt
``

or if you want to see already-added changes

``
git diff --cached myfile.txt
``

git log --graph --oneline<br/>

<br/>


``git commit <filenae>``
``git commit --ammend`` - change last commit

## Navgiation though the commit history

``git log`` - Show commit logs<br/>

To scroll down through the log, press:
- ``j`` or ``↓``<br/>
- ``d`` to move by half the page screen<br/>
- ``f`` to move by a whole page screen to scroll up<br/>
- ``k`` or ``↑`` to move up one line at a time<br/>
 u to move by half the page screen<br/>
- ``b`` to move by a whole page screen<br/>
- ``q`` to quit out of the log<br/>

``git log -p <file>`` - Show changes over time for specific file<br/>
``git blame <file>`` - Show who changed the code and when it was done<br/>

``git log --all --grep='commit message sample'`` - Find commit using commit message<br/>


 ``git log --oneline`` - displays short SHA and the commit message<br/>
``git log -2`` - show commits form last two days<br/>
``git log --since="2 days ago"``<br/>
``git log --before="2017-03-01"``<br/>
``git log --after="2017-03-01"``<br/>
``git log --author="Paulina"``<br/>

``git log --stat`` - shows which lists of the files that were changes as well as the number of added/removed lines



# Check difference between Commits
``git diff`` - see changes that have been done between commits or branches
``git diff --staged`` -
``git diff b48gabb..fc92rkr``

### Git Checkout
``git-checkout`` - Switch branches or restore working tree files

``git rm filename`` - remove filename


``git remove``
``git mv``

# Rebase



# REFERENCES
- https://en.wikipedia.org/wiki/Git
- https://app.pluralsight.com/library/courses/how-git-works/table-of-contents
- https://www.safaribooksonline.com/library/view/essential-git-/200000006A0403/
- https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Checking-the-Status-of-Your-Files
- https://www.atlassian.com/git/tutorials/inspecting-a-repository
- https://www.safaribooksonline.com/library/view/complete-git-and/9781789137293/
- https://git-scm.com/book/en/v2
- https://blog.osteele.com/2008/05/my-git-workflow/
