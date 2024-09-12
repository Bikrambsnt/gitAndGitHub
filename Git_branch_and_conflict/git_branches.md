# Git branches

it is like doing lots of work at a same time on a different environment without effetcing other's work environment.

Git branches provide same option 
it has a main or matser branch from where we can create other branches also to work on different projects whch will not affect any branches untill we merge it.

branches can craete on any branch either from main or from its childerns


There is a pointer which is called as a [head] it will always ponint to th head of the current working branch so that it can track whats going on on that file


# cmd

 <!-- To chech the current Branch -->

 git branch
 
 it will show the branch name with * astrick on it which is a head a ponter.

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

