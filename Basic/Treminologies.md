
# Commands
  ## Basic CMD

  git --version  
  <!-- Used t check the current version Of a Git -->

  git status
  <!-- Used to ckeck the current status of git -->

  git config --global user.email "example@gmail.com"
  git config --global user.name "Your name"
  <!-- This is used to config your email and username on the git while commiting the code or getting its git log -->

 git config --list
 <!-- This will show the changed settings which you have made -->

  git status
  git init
  <!-- It will create a git folder inside yor machine which contain the git information -->

  ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

  ## commit

  commit is used to save the work you have done by commiting the message 

  it has 3 rule that is

                        -----------             ------------          ------------
                        |  write  |   ------>   |   Add    | ------>  |   Commit |
                        |         |             |          |          |          |
                        -----------             ------------          ------------

 ## Git Flow

  Most important to understand what will happens when we add,or commit to git


    git init [Working Directory]---> git add [staging area] ---->git commit[repo] ---->git push[github]


   #### git init
        git init will create the working directory where we want to work linke in my case its folder<name one>

   ### git add

        it will create a staging area which means everything gets set to work but woking is not started yet but ready to work

        it has two area staging and unstaging area

  ### git commit

        it will will take us to repo [a folder] which save the work what we have done with a message.

  ### git push

        now till git commit the process is going only in our machi so git push will publish that work online which means now we are sharing and storing that work online.
    


  # commit cmd

  ##### git init

          for git init cmd will be

          git init

  #### git add
       git add <filename>
     <!-- or we can directly add all file using . -->
       git add .

  #### git commit

  git commit -m "Your message"

  git log
  <!-- git log wll display the current change or commit messages -->
   we can do git log --oneline to directly jump into the commit messages


  <!-- -m refers to the message that we want to say -->

<!-- Now till here you have initalize git add your file and dome commit -->





# git ignore

.gitignore is a special file which is used to hide the sensetive data or modules to get published with others while pushing

git ignore will simply ignore the file that is added inside it

  .git ignore
   node_modules
   .env


   