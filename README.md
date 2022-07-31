This is GIT practice 

git status 
git add . --> adding into staging area
git add nameOfFile

git commit --> get all from stage area and then commit their changes

git config --global user.name "name"
git config --global user.email "name@name.com"

git log --> to get log of changes

git remote add [Name (origin)] repoAddress
origin = your remote git repository 

git push [--set-upstream] origin master
all these configuration are stored on .git folder , if you remote it, the connection/git init will be lost

git branch --> to get list of branches
git pull --> to get latest changes
git checkout nameOfBranch
git checkout -b newBranch --> create new branch and switching to newBranch 

we have dev branch and master branch 
dev branch is intermediary master, it's tested and features and bugfixes add into dev branch and end of sprint it will be added to the master

only master branch is considered for continuous integration/delivery 

Merge Requests
big feature , junior developer or expertise in different area 
junior developer or expertise in different area 
must be in stable version


Delete branches after go to master and pull first

git pull -r (rebase) --> to not get merge those new commit and replace my own commit overwrite the merge one (on top)
then do the git push ..so avoid those unnecessary commit

git branch -d [nameOfBranch]

