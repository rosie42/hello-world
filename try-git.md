Using the Try Git tutorial from codeschool.com

create a repo 
git init

this creates and an empty repo /.git/ in the current directory

get the current status of the repo 
git status

start tracking the test file to the repo
git add octocat.txt

commit the changes to the repo and add a comment
git commit -m "Add cute octocat story"

wildcard additions
git add '*.txt'

browse changes
git log

add a remote repo to github
git remote add origin https://github.com/try-git/try_git.git

push local repo (and changes) to github repo (origin [master branch])
git push -u origin master

pull from remote repo
git pull origin master

get the diffs, most recent commit is HEAD
git diff HEAD

compare changes between staged and commited files
git add octofamily/octodog.txt
git diff --staged

unstage files using the git reset
git reset octofamily/octodog.txt

go back to last commit for file octocat.txt with git checkout
git checkout -- octocat.txt

create a branch to clean up the master
git branch clean_up

view the different branches 
git branch

switch to the clean_up branch with git checkout
git checkout clean_up

delete files and stage the files for removal from the repo
git rm '*.txt'

commit the removal
git commit -m "Remove all the cats"

switch back to the master
git checkout master

merge the clean_up branch
git merge clean_up

delete the clean_up branch
git branch -d clean_up

push everything back to the remote repo
git push