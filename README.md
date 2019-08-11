-maybe I should make this its own repository and have it uploaded to github so I can switch
between computers at any given point but have access to my notes
-but the real question is do I want this to be a different file type like a word document so I can
have fancier features for organizing my text and such

git status
-you are going to be using 'git status' a lot when as you will need to know and make sure you know
-what is on the chopping block for being pushed and added to the repository
lets you know which files will be commited
-shows which files will be commited and which ones won't be
-shows untracked which means files that won't be commited to the master and such I think
-if you make changes to a file, then check the status, it will have a new section called
'Changes not staged for commit' which tesll you 'hey these changes won't be commited but exist' 
when its not being commited its called to be in the staging area

git add
-adds a file to the commit folder which you can upload
-you can use *.'filetype' in order to add all files to the 'to commit' status
-too add everything you 'do git add .'

git rm --cached 'filename'
removes the file from those that are going to be uploaded/commited

git init
im not sure what this exactly does but it creates a .git folder with a bunch of things
in whatever folder you are looking at
my guess is that this needs to be present in order to use git for whatever project you are are
working on

git commit
-on windows it will be a vim editor so you have to jsut go into insert mode 'i' and then remove the commented out 'Initial commit' then 'esc' then ':wq' to save and quit
-on linux you don't have to go on insert mode like with vim, go in uncomment 'Inital commit', then you do ctrl+O and that will write to disk aka save files, then exit and it should give you commit message
-'git commit -m 'changed app.js' this is hw you skip the whole editing stage and add the commit onto what changes you have maded

git ignore
-by doing this you make it so the file can never be added to the commit list
-you have to create this document by doing 'touch .gitignore' or through an editor app and saving as
-then in the .gitignore file you just list anyting you don;t want pushed,
-you can ignore entire directories as well
-you could also just block entire types of files

branches
-instead of commiting to the main project file, aka the master, you create a copy that you commit to for all to see and testing purposes and then decide what to do from there
-git status also lets you know which branch you are on

git checkout 'branch name'
-this lets you switch branches in your repository
-if you are lookign at the files, you can add something to the nonmaster branch, commit it, then switch between the two to see that there is indeed a difference between the branches content
-you can merge to make the branches the same

git merge 'branchname'
-lets you merge the master and the specified branch

linking to github?
-so we have created the repository locally but its not attached to the github account so we gotta change that by going onto the github website and creating a repository there
-so the command is git remote add origin 'website url'
-one the video he copy and apsted from github but it is not showing me but from what i undestand it is jsut the url when you are on the code portion of the repository
-after that it will say origin which means ...
-well first you have to do one more step which is git push -u origin master
-this pushes it to the repository and then you have to login which sucks cause i never remember my password the first time since i have so many variations
-so when you do create the repository on github, you will have the option to have a readme, if you do this and then you try to push wihotu one in your reposiroty it will give an error due to differences so don't do this and have to remove the remote

git remote rm 'remote name'
-removes the remote in case it changes or I mess up

don't forget to add the comment after the git commit -m to say what you changed



