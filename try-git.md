Using the Try Git tutorial from codeschool.com

create a repo 
```bash
git init
```

this creates and an empty repo /.git/ in the current directory

get the current status of the repo 
```bash
git status
```

start tracking the test file to the repo
```bash
git add octocat.txt
```

commit the changes to the repo and add a comment
```bash
git commit -m "Add cute octocat story"
```

wildcard additions
```bash
git add '*.txt'
```

browse changes
```bash
git log
```

add a remote repo to github
```bash
git remote add origin https://github.com/try-git/try_git.git
```

push local repo (and changes) to github repo (origin [master branch]). The `-u` flag causes git to remember the options
```bash
git push -u origin master
```

pull from remote repo
```bash
git pull origin master
```

get the diffs, most recent commit is HEAD
```bash
git diff HEAD
```

compare changes between staged and commited files
```bash
git add octofamily/octodog.txt
git diff --staged
```

unstage files using `git reset`
```bash
git reset octofamily/octodog.txt
```

go back to last commit for file octocat.txt with `git checkout`
```bash
git checkout -- octocat.txt
```

create a branch to clean up the master
```bash
git branch clean_up
```

view the different branches 
```bash
git branch
```

switch to the clean_up branch with `git checkout`
```bash
git checkout clean_up
```

delete files and stage the files for removal from the repo
```bash
git rm '*.txt'
```

commit the removal
```bash
git commit -m "Remove all the cats"
```

switch back to the master
```bash
git checkout master
```

merge the clean_up branch
```bash
git merge clean_up
```

delete the clean_up branch
```bash
git branch -d clean_up
```

push everything back to the remote repo
```bash
git push
```
