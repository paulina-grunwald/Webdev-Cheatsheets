git hash-object --stdin


We have following __git objects__:
- Blobs,
- Trees,
- Commits
- Annotated Tags.

Every object in Git has its own SHA1.

``-a`` - hidden<br/>
``-t`` - type<br/>
``-p`` - pretty print<br/>
``ls`` -  print all files in the folder<br/>


``git branch`` - check the list of branches
``git init`` - Initialize empty git repository in selected folder<br/>
``git status`` - check status<br/>
``git add`` - add files to staging area<br/>
``git commit -m "First commit"`` - commit the file with the commit message<br/>
``git log`` - check the list of existing commits<br/>

``git count-objects`` - count objects in the git repo<br/>

``ls -a`` - view all hidden files in the repository

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



# REFERENCES
- https://app.pluralsight.com/library/courses/how-git-works/table-of-contents
