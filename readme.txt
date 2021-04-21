-- workspace => stage
git add readme.txt

git status

-- stage => git_local
git commit -m "git command list"

-- show git log
git log

-- show git command log
git reflog


-- remote related command 
git remote add origin https://github.com/miningant/HelloWorld.git
git remote -v

git config --global credential.helper store
git remote set-url origin git@github.com:miningant/HelloWorld.git


-- git_local => git_remote
git push origin master

--Creating a new branch is quick.
git checkout -b dev
git branch

--update readme and commit to branch dev
git add readme.txt
git commit -m "commit to branch dev"

-- switch branch to master, readme is different
git checkout master

-- merge branch dev to master
git merge dev