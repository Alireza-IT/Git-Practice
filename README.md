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

for fixing the conflict we have to git rebase --continue after solving the conflict

.gitignore--> we have to put build folder when compile code is needed so we need to put these files into .gitignore 
build/*
also best case is to not consider the dependencies file as well 
git rm -r --cached [name of file or folder] if we want to ignore one file which already has been tracked by git.

if having changes in this branch , need to move another branch but do not want to commit these changes because these changes are under process, so changing branches will be forbidden.
so we do 
git stash --> to save our changes and hide them to git and we are able to change branch 
git stash pop
another way we can hide changes to see if the application work without my changes or not (in case of doubts)

History/Logs commit 
useful for testing 
we can checkout the commit and we are going back to application 
git checkout [commithash] and we are in detached head
we can create new branch based on these point of code (not very common way)
go back to up to date state 
git checkout nameofbranch 


