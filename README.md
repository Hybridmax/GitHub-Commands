# Create New Repository

git init    <-- initialize empty repository

git add .    <-- Add your Project (or new added files) to your Repository

git commit -m "commit message"    <-- commit your changes

git remote add origin https://github.com/Hybridmax/Hybridmax-Kernel-I9505    <-- add your github url

git pull origin master    <-- merge your project from github to you local repository of your computer

git push origin master    <-- upload your changes to github
###############################################################################

# Create New Branch

git checkout -b branchname    <-- New Branch

git push origin branchname    <-- Push the branch on github

git branch    <-- You can see all created branches

git remote add remotename    <-- add a remote to your branch

git push origin remotename    <-- Push changes from your commit into your branch

git fetch remotename    <-- Update your branch when the original branch has been updated

git merge remotename    <-- Then you need to apply to merge changes

git branch -d branchname    <-- Delete a branch on your local filesystem

git branch -D branchname    <-- To force the deletion of local branch on your filesystem

git push origin branchname    <-- Delete the branch on github
###############################################################################

# update & merge

git pull origin master

git merge branchname

git add .

git commit -m "commit message"

git push origin master
###############################################################################

# Cherrypick commits from other repositorys of other developers or another repository from you

for example: @slim80 don't hate me for this :-)

git remote add slim80 https://github.com/Slim80/Imperium_Kernel_TW_4.4.2

git fetch slim80

now you have added the other repository to you repository (no one can see that)

now go to the repository that you have fetched and click on any commit you want to cherrypick

in top right of the page you see a long line of numbers. this is the commit

copy the first 8 numbers and type following for example:

git cherry-pick 12345678    <-- this is the cherrypick

[git cherry-pick]    <-- this is the cherrypick command [12345678]    <--this is the commit

git push origin master    <-- upload your cherrypicked commit to your repository
###############################################################################
# revert a commit that for example includes any errors

git revert 12345678    <-- revert a commit of your repository
