## What is origin/main?

A remote tracking branch, despite that the word remote appears its name, is actually not remote, it is completely local to your local Git repository. It's main purpose is to serve as a proxy for the actual branch which exists on the remote (e.g. GitHub, Bitbucket, etc.).
It is local copy of the branch named "main" on the remote named "origin".The origin/main branch is local! Any time you fetch from origin, origin/main will get updated.The origin/main branch is not a reference or pointer to the main branch on origin. It is a local copy.

Since origin/main is a branch, you can merge it. Here's a pull in two steps:

- Step one, fetch main from the remote origin. The main branch on origin will be fetched and the local copy will be named origin/main.

`git fetch origin main`

- Then you merge origin/main into main.

`git merge origin/main`

- Then you can push your new changes in main back to origin:

`git push origin main`

## What does git fetch do?
It pull any new commit from remote to local origin/main branch. Its doesnt merge them with local main. to see the commit you need to merge origin/main to main branch.

-----
