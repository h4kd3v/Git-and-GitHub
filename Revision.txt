# Notes File

Revision Notes for Git and Github

Commands :

git status  (To see what we have changed in Local working copy)

git add .   (Track all file changes)

git commit -m "Header" -m "Message for the commit"  (Commit your local changes to GIT)

ssh-keygen -t rsa -b 4096 -c "test@gmail.com"   (Command to generate SSH keys)


// Save your public key under Github SSH key section.

Start ssh-agent in background and add your private key in terminal so you can push code anytime locally.

$ eval "$(ssh-agent -s)"
$ ssh-add ~/.ssh/githubSSHkeys/githubkeys

git push origin main            (Command to push your code in the main branch)

git init                    (Initialise the Git Repository)

git remote add origin  git@github.com:h4kd3v/repo1.git      (Add Reference of path as where to push this new local project)

git remote -v                      (View the new changes added by above command)

git push -u origin main            (Commit to the origin branch,also after using -u, in future u can only use $ git push )

git branch                          ( To see the branches, also * means currently on that branch )

git checkout -b feature-branch      ( Make a new branch )

git checkout main                   (Switch to main branch)

git merge feature-branch            (Merge the two branches, here feature and main branch)

git push -u origin feature-branch   (Push to specific branch)

git pull origin main                (Pull chnages in the main branch)

git branch -d feature-branch        (Delete an existing branch)

git diff                            (Shows changes made from last commit)

git diff main                       (Compare current branch's changes with main)

git commit -am "Added new commands"    (Adds and commits at same time, only works with modified, not newly created)

#Resolving Confilcts

git reset                           (Reverses Changes, unstages files)

git reset HEAD~1                    (Resverse the last one commit)

git log                             (View git logs)

git reset 25ae27ed3ae5caf1b409b76535bf8aa227791315    (Get back to a particular commit)

git reset --hard e19b1aef53cf8e9b99e3c72a8ba2b583a8ad887d       (Not only unstages files, but also reloves commited coded completely)
