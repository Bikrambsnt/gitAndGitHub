# Git branches

it is like doing lots of work at a same time on a different environment without effetcing other's work environment.

Git branches provide same option
it has a main or matser branch from where we can create other branches also to work on different projects whch will not affect any branches untill we merge it.

branches can craete on any branch either from main or from its childerns

There is a pointer which is called as a [head] it will always ponint to th head of the current working branch so that it can track whats going on on that file

# cmd

 <!-- To chech the current Branch -->

git branch

it will show the branch name with \* astrick on it which is a head a ponter.

 <!-- To create new Branch -->

git branch <branch name>
git branch

example git branch python

<!--  -->

<!-- To switch the branches -->

git switch <branch name>
git branch

examle git switch python

<!-- Switched to python branch -->

<!-- We can directly craete a branch and get instant switch to that using -->

git switch -c javaScript
git branch

<!-- if javaScript is already available then it will just switch to that Branch -->

<!-- to switch on other branch we can use checkout also, branch need to exist -->

git checkout <branch name>
git branch

example git checkout javaScript

<!-- Switch to javascript  branch-->

# merging

###### Fast forward Merge

Now when we work on different branch then that branch cannot be accessable by another branch like i am on master branch so I cant access python or javaScript branch so now to grt the access of that branch we have to merge it.

Merging a branch can be done from where the branch need to be merge .

#### cmd

    git merge <branch name>

example git merge python [while doing this I am on master branch]

<!-- This will merge the python branc on master branch-->

###### Non fast forward Merge

In this we work on aboth branch like in master and on python branch we will write add and commit on both branch but when we merge the branch from master branch then

merge conflict arrive
when merge conflit arrive it will ask for the another commit on terminal or on a code editor
we have to write the commit there also to fix the merge then close it to save.

cmd
git merge <branch name>

# Merge-Conflicts

merge conflict arrive when we work on same file from defferent branches
like i have a merge-conflict.txt file on that file I have wrote some lines of txt from both the branches as it will work on independent environment so python branch is unknown that I have added some lines of txt on master branch and master branch is also unknown that I have added some points on python branch

now conflict arrive when I try to merge it

git merge pthon

         Now when conflict happens it display like this


        ----------------------------------------------
         |                                           |
         |   <<<<<<<<< HEAD                          |
         |     -----------------                     |   ------> Branch That you are on(master)
         |      ----------------                     |
         |        ----------------                   |
         |                                           |
         | =======================================   |
         |  ------------------------                 |
         |     -----------------------               |
         |         --------------------              |
         |     >>>>>>>>>>>>>>> <branch name>         | ------> conflict that came from another
         |                                           |                           Branch (python)
         |-------------------------------------------|

        In this Head is refer to the current wroking branch and down one is the conflicted branch

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Now to fix this conflict we will do some steps

###### Step 1

    git status
    git merge --abort [this will abort the current merge]

###### step 2

    git merge <branch>
    git merge python

    now lets Manually resolve it
      first go to merged file to resolve it

##### step 3

To resolve it manually we have to remove file contain which is not so important as we think

so just erase that part along with head and bottom greater than sign.

after that just save the file

the use cmd

git status

git add <file name>
git commit -m "Commit message"

Here we finally resolved our git merge confilct problem.

###### Rename branch
    git branch
  git branch -m <old-brach-name> <new-branch-name>
example git branch -m <javaScript> <javaScript-DSA>

###### Delete Branch

 git branch -d <branch name>
 example git branch -d newBranch
 git branch
