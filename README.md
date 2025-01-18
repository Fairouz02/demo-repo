# Demo

delete once done

## End of tutorial keynotes

### Cloning Repo until pushing commit up to Github
clone repo from github: git clone ~ssh~
adding a new file that was not a part of the commit: git add . or git add ~name of file~
comitting: git commit -m "Message" -m "Optional Desc"
combining add and commit: git commit -am "Message"
pushing commit to github: git push origin ~name of branch~

### Pushing folder created locally to github
initialise the created folder: git init
continue with the folder until ready to push to github repo
create repository in github and add folder. get the repo ssh.
connect the local folder and online repo: git remote add origin ~repo ssh~
push the folder into the online repo

### Branch
create branch: git checkout -b ~name of branch~
navigate branch: git checkout ~name of branch~ 
current branch: git branch
pushing to github a branch that was created locally: git push -u origin ~name of branch~
after pushing branch on github, merge the codes in github
once merged, pull the updated codes from master branch by executing: git pull
remove branch when its legacy: git branch -d ~name of branch~

### Merging Locally
local merging is done to keep the user up to date. not the team. example, touching up the current feature with the most up to date master branch
merging the feature branch into the master branch locally: git merge master
deconflict the lines of codes directly in code editor after merge

### Undoing 
unstaging changes (reseting): git reset ~optional name of file~
undoing a commit: git reset HEAD~1 ("HEAD" is a pointer to the last commit. ~1 means to jump 1 additonal previous commit)
view logs of commit: git log
to return to a unstaged version of a specific commit log: git reset ~hash of commit from the log~
return to the inital version of a commit version: git reset --hard ~has of commit from the log~