# exercise1


1. create repo on github
2. make clone repo in local folder 


stape 1:
 -> create new branch develop
    - git checkout -b develop

 -> create new branch branch1
    - git checkout -b branch1

stape 2:
 -> got to .git/hooks/commit-msg.sample
    - remove .sample
    - add echo "commit message hook run successfully" line on top

 -> run command 
    - chmod u+x .git/hooks/*

stape 3: 
 -> perform multipal commit on branch1
    - modify sumthing and run command given bellow

    - git add .
    - git commit 

stape 4:
 -> push both branch develop and branch1 on github
    - git push origin develop
    - git push origin bransh1

    - now show pull request created on github 

stape 5:
 -> go to develop branch 
    - git checkout develop

 -> create new branch branch2 
    - git checkout -b branch2

stape 6:
 -> commit something in ranch2
    - modify file 
    - git add .
    - git commit

 -> push branch2 on git hub
    - git push origin branch2

 -> during this time merge alredy created pull request branch1 in to develop on git hib
    - go to github 
    - creat PR
    - select develop as base and branch1 as second
    - merge bot branch 

stape 7: 
 -> Create a PR for the current branch, given your branch should be up to date with develop branch
 






 