## for the original

- `git init `: lets you initialize Git in your folder.

- `git add Readme.md` lets you add the Readme file, while `git add .` lets you add all files in the present folder.

- `git status`

- `git commit -m "This is my first commit!"` : stores the added files. Use `-m` for message followed by the actual message.

- `git checkout -b branchName`

- `git branch`
- `git merge testbranch`

-` git remote add origin https://github.com/amjarino/learn-git-github.git` : connects the local folder to the repository on GitHub. It is followed by the repository's link.

- `git branch -M main` : creates a new branch which is a new version of the repository as it appears when added, and `-M` to move the name to main.

- `git push -u origin master/main` : pushes the code to GitHub. The -u flag creates a tracking reference for the branch, and origin main puts the code in the main branch.
- `git push origin my-new-branch`

- `git pull origin master`
- `git log`

## for contrubtions :

1. Git GitHub Fork repo
2. clone the original repo

- `git clone https..`
- Creating a branch to work on:

  > Before making changes to the project, you should create a new branch and check it out. By keeping changes in their own branch, you follow GitHub Flow and ensure that it will be easier to contribute to the same project again in the future.

`git  branch branchname `
`git checkout branchname`

3. Configuring Remotes :

- `git remote rename origin upstream`
- `git remote add origin https://myfork.repo`
- `git add .`
- `git commit -m "a short description of the change"`

4. `git push origin`

- Check that your fork is the "origin" remote
  - `git remote -v`
    if not setb it
    - `git remote add origin URL_OF_FORK`.
- Add the project repository as the "upstream" remote
  > Go to your fork on GitHub, and click the "forked from" link to return to the project repository:
  > Add the project repository as the "upstream" remote using:
- `git remote add upstream URL_OF_PROJECT`.
- Pull the latest changes from upstream into your local repository

> Before you start making any changes to your local files, it's a good practice to first synchronize your local repository with the project repository. Use git pull upstream master to "pull" any changes from the "master" branch of the "upstream" into your local repository. (If the project repository uses "main" instead of "master" for its default branch, then you would use git pull upstream main instead.)

> If you forked and cloned the project repository just a few minutes ago, it's very unlikely there will be any changes, in which case Git will report that your local repository is "already up to date". But if there are any changes, they will automatically be merged into your local repository.

### Create a new branch :

Rather than making changes to the project's "master" branch, it's a good practice to instead create your own branch. This creates an environment for your work that is isolated from the master branch.

Use` git checkout -b BRANCH_NAME` to create a new branch and then immediately switch to it. The name of the branch should briefly describe what you are working on, and should not contain any spaces.

For example, I used `git checkout -b doc-fixes` because I was making some small fixes to the

### Commit your changes

After you make a set of changes, use git add -A to stage your changes and `git commit -m "DESCRIPTION OF CHANGES`" to commit them.

For example, I used `git commit -m "fix typos in set_config docstring`" for one of my commits.

If you are making multiple sets of changes, it's a good practice to make a commit after each set.

### Push your changes to your fork

When you are done making all of your changes, upload these changes to your fork using` git push origin BRANCH_NAME`. This "pushes" your changes to the "BRANCH_NAME" branch of the "origin" (which is your fork on GitHub).

For example, I used `git push origin doc-fixes`

### Begin the pull request

5. Go to GitHub, and we see that the repository has a new commit. And we can send a Pull Request to the original repository.
6. create a pull request

## Approving Pull Requests :

> Now any member with access can see the Pull Request when they see the original repository, And they can see the proposed changes, Comment on the changes and merge, confirm merge and voila...
