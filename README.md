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
    - git checkout develop
    - git pull origin developo
    - git checkout branch2
    - git rebase develop
    - git push origin branch2

 -> now auto maticly create pR which is upto date with develop branch 

stape 8:                                                             

 -> add some tage 
    - git tag [tag name]
    - git push origin [tag name]
    - git tag [tag name ] [commit sha]

stape 9:                                                                

 -> Create 2 another branch (branch3 and branch4) from develop
    - git checkout develop 
    - git checkout -b branch3
    - git checkout develop 
    - git checkout -b branch4

stape 10:       

 -> add commit somthing on branch3
    - git checkout branch3
    - git commit

stape 11:     

 -> Cherry pick branch3 branch's commit to branch4 branch.   
    - git log --oneline
    - copy last sha 
    - git checkout branch4
    - git cherry-pick [sha]

stape 12:                      

 -> change commit mesage in branch4      
    - git checkout branch4
    - git commit --amend -m "new mwssage"

stape 13:                                                       
                                                   
 -> add 3 commit on branch4

 -> remove last commit 
    - git reset HEAD~1
    - git reset HEAD~1
    - git commit new
    - git push --force origin branch4
    
 






 