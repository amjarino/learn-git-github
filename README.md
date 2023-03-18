# Learn Git and Github (2019)

## for the original

- git init : lets you initialize Git in your folder.

- git add Readme.md lets you add the Readme file, while git add . lets you add all files in the present folder.

- git status

- git commit -m "This is my first commit!" : stores the added files. Use -m for message followed by the actual message.

  git checkout -b branchName

- git branch
- git merge testbranch

- git remote add origin https://github.com/amjarino/learn-git-github.git : connects the local folder to the repository on GitHub. It is followed by the repository's link.

- git branch -M main : creates a new branch which is a new version of the repository as it appears when added, and -M to move the name to main.

- git push -u origin master/main : pushes the code to GitHub. The -u flag creates a tracking reference for the branch, and origin main puts the code in the main branch.
- git push origin my-new-branch
  jib
- git pull origin master
- git log

## for contrubtions :

1- Git GitHub Fork repo
2- clone the original repo

- Creating a branch to work on:

  > Before making changes to the project, you should create a new branch and check it out. By keeping changes in their own branch, you follow GitHub Flow and ensure that it will be easier to contribute to the same project again in the future.

  `git  branch branchname
`git checkout branchname
  3- Configuring Remotes :

- git remote -v
- git remote rename origin upstream
- git remote add origin https://myfork.repo
  4- git push origin
  5- Go to GitHub, and we see that the repository has a new commit. And we can send a Pull Request to the original repository.
  6 - create a pull request

  ***

  ## Approving Pull Requests :

  Now any member with access can see the Pull Request when they see the original repository, And they can see the proposed changes, Comment on the changes and merge, confirm merge and voila...
