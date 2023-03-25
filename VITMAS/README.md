These are a list of few commands are used frequently on Github (git bash):

git help
Take help from github help section for different commands and other errors.

git config
To set the basic configurations on github like your name and email.  

git config –-global user.name “XYZ”
Sets configuration values for your user name on git. 

git config –-global user.email xyz@gmail.com
Sets configuration values for your user email on git.

git config –-global color.ui true
To see different colours on command line for different outputs.  

mkdir store
Create a directory if not created initially. 

cd store
To go inside the directory and work upon its contents.

git init
To create a local git repository for us in our store folder.This will help to manage the git commands for that particular repository.

git status
To see whats changed since last commit.It shows all the files that have been added and modified and ready to be committed and files which are untracked.

git add Readme.txt
To add a file Readme.txt to the staging area to track its changes.

git commit -m “Created a Readme.txt”
To commit our changes (taking a snapshot) and providing a message to remember for future reference.

git log
To check the history of commits for our reference.

git add
To add a specific list of files to staging area.

git add --all
To add all files of current directory to staging area.

git add *.txt
To add all text files of the current directory to staging area.

git add docs/*.txt
To add all text files of a particular directory(docs) to staging area.

git add docs/
To add all files in a particular directory(docs) to staging area.

git add “*.txt”
To add text files of entire project to staging area.

git diff
To figure out what changes you made since last commit.

git reset head license
To undo staging of the file that was added in the staging area.

git checkout –license
To Blow away all changes since the last commit of the file.

git commit -a -m “Readme.md”
To add any of our tracked files to staging area and commit them by providing a message to remember.

git reset –soft HEAD^
To undo last commit and bring file to staging area.

git reset –hard HEAD^
To undo last commit and remove file from the staging area as well(In case we went horribly wrong).

git reset –hard HEAD^^
To undo last 2 commits and all changes.

git remote add origin https://github.com/xyz/MyAlgorithms.git
Makes a bookmark which signifies that this particular remote refers to this URL. This remote will be used to pull any content from the directory and push our local content to the global server.

git remote add <address>
To add new remotes to our local repository for a particular git address.

git remove rm
To remove a remote from our local repository.

git push -u origin master
To push all the contents of our local repository that belong to master branch to the server(Global repository).

git clone https://github.com/xyz/MyAlgorithms.git
To clone or make a local copy of the global repository in your system (git clone command downloads the repository and creates a remote named as origin which can be checked by command – git remote -v).

git branch Testing
To create a new branch named as Testing.

git branch
To see all the branches present and current branch that we are working on.

git checkout Testing
To switch to branch Testing from master branch.

ls
To see directories and files in the current directory.

ls -la
To see hidden directories and files with in the current directory.

git merge TestingTo merge Testing branch with master branch.

git branch -d TestingTo delete Testing branch.  

git checkout -b admin
To create a new branch admin and set it as current branch.

git branch -r
To look at all the remote branches.

git branch -D Testing
To forcefully delete a branch without making commits.  

git tag
To see the list of available tags.

git checkout v0.0.1
To set the current tag to v0.0.1

git tag -a v0.0.3 -m “version 0.0.3”
To create a new tag.

git push –tags
To push the tags to remote repository.

git fetch
To fetch down any changes from global repository to current repository.

git stash
To move staged files to stash area which are present in staging area.

git stash pop
To get back the files which are present in stash area.

git stash clear
To clear the stash folder.

git rebase
Three tasks are performed by git rebase:
  - Move all changes to master which are not in origin/master to a temporary area.
  - Run all origin master commits.
  - Run all commits in the temporary area on top of our master one at a time, so it avoids merge commits.
