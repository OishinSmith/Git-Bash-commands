# Git-Bash-commands
A list of useful commands for the Git Bash terminal that I use commonly

# Commands

`git status`

tells you what branch you are in eg:

>>git status
On branch master
nothing to commit, working tree clean


`git config --global user.email "oishin.smith@gmail.com"`

you need to do this so that github knows who you are, it causes errors if you dont

`git init`

You need this to initialise the local directory as a Git repository

`git add .`

Adds the files in the local repository and stages them for commit.

`git commit -m "adding the exercises to github from the git command line"`

Commits the tracked changes and prepares them to be pushed to a remote repository. You can also add a comment at the end.

`git remote add origin https://github.com/OishinSmith/Python-exercises.git`

Sets the new remote. This is the location where you want the files to be pushed to

`git remote -v`

Verifies the new remote URL. an example message displayed will be: 
>>origin  https://github.com/OishinSmith/Python-exercises.git (fetch)
>>origin  https://github.com/OishinSmith/Python-exercises.git (push)

`git push origin master`

Pushes the changes in your local repository up to the remote repository you specified as the origin which is your github repository called:
>>https://github.com/OishinSmith/Python-exercises.git
in this example.

if you ever get the error code 
>>"error: failed to push some refs to 'https://github.com/OishinSmith/Python-exercises.git'"
use `git push origin master -f` to solve the problem since it uses "force"
