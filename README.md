# git-docs

## Some simple commands

* Git clone with a specific branch with a new name
```bash
git clone https://github.com/RTGW-group/RTGW2020.git rtgw2020-v2.8.5 --branch multicuda    
```

* Add the original remote server to you local repo 'git cloned' for a fork
```bash
git remote -v
git remote add upstream https://github.com/RTGW-group/RTGW2020.git
git remote -v
```

* Checkout a branch or create a new branch
```bash
git branch
git checkout multicuda
git checkout -b multicudaNew
```

* Push a new local repo to remote server as a new branch
```bash
#assume that we have a new local repo with the name of 'multicudaNew',
#but we want to push it to the remote server as a new branch with new name of 'multicudadev'
git push origin multicudaNew:multicudadev
```

* Update a branch with the remote server, there is a safe way
```bash
git fetch origin main:tmp
git merge tmp
```

* Removes the copy of the file from the staging-area under the senario that you have staged a file you do not want to. The n you can execute this one before you add and commit once again.
```bash
git rm -r --cached . 
```

* Revert to a previous commit ID
```bash
git reset --hard commit_id
```

## Workflow for contribution to RTGW-group.

 
