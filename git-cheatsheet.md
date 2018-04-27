# Git Cheat Sheet
> by Paulina Grunwald

__VCS/VCM__ - version control systsem/source code manager

__File status lifecycle__ - movement of the files bewteen stages in the git. Files can be in 4 various stages: ``untracked``, ``tracked``, ``modified``, ``staged``.

__SHA__ - ID number for each commit. Each SHA is unique

__Branch__

We have following __git objects__:
- Blobs,
- Trees,
- Commits
- Annotated Tags.

Every object in Git has its own SHA1.

``pwd`` -  present working directory<br/>
``mkdir your_folder_name`` -  create new folder
``cd your_folder_name`` - change directory
``rm`` - remove files and directories

Flag is used to alter how a program functions

``-a`` - hidden<br/>
``-l`` - view details of the file<br/>
``-t`` - type<br/>
``-p`` - pretty print<br/>
``ls`` -  print all files in the folder<br/>
``ls -al`` - get all the files including hidden file and their details

``git branch`` - check the list of branches<br/>


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

git log --graph --oneline

### Navigation through the log
``git log`` -Show commit logs

To scroll down through the log, press:
- ``j`` or ``↓``
- ``d`` to move by half the page screen
- ``f`` to move by a whole page screen to scroll up, press
- ``k`` or ``↑`` to move up one line at a time
 u to move by half the page screen
- ``b`` to move by a whole page screen
- ``q`` to quit out of the log


Find commit using commit message:
git log --all --grep='commit message sample'
 ``git log --oneline`` - displays short SHA and the commit message

``git log --stat`` - shows which lists of the files that were changes as well as the number of added/removed lines
# REFERENCES
- https://app.pluralsight.com/library/courses/how-git-works/table-of-contents
- https://www.safaribooksonline.com/library/view/essential-git-/200000006A0403/
- https://git-scm.com/book/en/v2/Git-Basics-Recording-Changes-to-the-Repository#Checking-the-Status-of-Your-Files
- https://git-scm.com/docs/git-status
- https://www.atlassian.com/git/tutorials/inspecting-a-repository
