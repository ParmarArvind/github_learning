<!--  rebaseing (same as merge branches)-->    
git rebase branchName // if you are in payment branche and you want to rebase it after the master branch then use it , it add the payment branch after the master branch
//after rebse 
    git status
    git add . // don't commit it 
    git rebase --continue // if confilict occur and something is comes in terminal then wre you cna change the commit messages use i key then change the commit message the for exit :wq 
// at the end merge it with master
git merge branchName
 
<!--  github push and pull 
never push main branch to github use another branch to pull in real projects-->    

    
    <!-- git basic -->

git init
// initialize git repository

git status
// check current status

git add .
// add all files

git commit -m "message"
// save changes

git branch
// show branches

git checkout master
// switch to master branch

git checkout payment
// switch to payment branch

git checkout -b payment
// create + switch branch

git branch -D payment
// delete branch


<!-- merge -->

git merge payment
// merge payment branch into current branch

// after conflict
git status
git add .
git commit -m "merge completed"


<!-- rebase -->

git rebase master
// move payment branch after latest master commits

// after conflict
git status
git add .

git rebase --continue
// continue rebase after fixing conflict

git rebase --abort
// cancel rebase

git rebase --skip
// skip conflicted commit


<!-- github -->

git remote add origin repositoryLink
// connect github repository

git branch -M main
// rename branch to main

git push -u origin main
// first push to github

git push
// push latest changes

git pull
// pull latest changes

git pull origin
// pull from origin

git pull origin main
// pull latest changes from main

git push -u origin pay
// first push of pay branch


<!-- useful -->

git rev-parse --show-toplevel
// show repository root folder

git restore fileName
// discard changes from file


<!-- editor -->

git config --global core.editor "code --wait"
// set VS Code as git editor