# Git Stash

    This is the method to store the staging area process without commiting

    if I am on staging area and want to visit anither branch then I can use stach method to hold it for some time without commiting the code.

#### cmd
     
        git stash

###### Naming stash

    we can name the stash too
       git stash save "Work In progress"

###### list Stash

        git stash list

###### apply the stash

    git stash apply


###### apply the specific stash

git stash apply stash@{0}


###### To apply and drop the Stash at a same time
  
   git stash pop

###### Drop stash

 git stash drop


 ###### Applying stash at a particular branch

 git stash apply stash{0} <branch name>

 ###### Clearing the Stash

 git stash clear