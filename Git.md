## Git
  * [awesome-cheatsheet](https://github.com/arslanbilal/git-cheat-sheet#readme)

## Log
  - git log
  - git log -2
  - git log --oneline
  - git log --stat
  - git log -p
  - git log -p master..branch_name
  - git log --merges --oneline
  - git log --author="mehultilala"
  - git log --grep="ignore"
  - git log --pretty=format:'%cn %h'
  - git log --pretty=format:"%ad %h by %an, %s" --date=iso | sort -r | less

## personwise commits
  - git shortlog
  - git shortlog -n
  - git shortlog -n -s
  - git shortlog -n -s -e

## reset to  hard=> no changes are preserved, soft: changes reserved as staged, default=> changes preserved as unstagged
  - git reset hash
  - git reset HEAD~1
  - git reset --soft hash
  - git reset --hard hash

## reverts commit and creates revert commit
  - git revert hash

## amend commit
  - git commit --amend -m "message"
  - git commit --amend --author ="message"
  
## view commit
  - git show #
  - git show --pretty="" --name-only #
  
## stash commands
  - git stash save "custom_name"
  - git stash list
  - git stash pop stash@{n}
  - git stash apply stash@{n}

## set remote
  - git remote set-url origin git@github.com:keshav-truckola/truckola.git

## pick single commit from other branch
  - git cherry-pick hash
  - git cherry-pick hash --no-commit

## log of operation performed on dev
  - git reflog

## garbage collection
  - git gc

## merge all commits in branch to single
  - git rebase -i hash (basehashofbranch)

## Branch
  - git branch
  - git log master..
  - git cherry -v master

## create new branch and push changes flow
  - git pull origin master
  - git checkout -b branch_name //create local branch
  - git commit -am 'message'
  - git push origin branch_name

## checkout existing remote branch and push changes flow
  - git pull
  - git checkout remote_branch_name
  - git commit -am 'message'
  - git push origin remote_branch_name
  - git show --stat --oneline HEAD

## changed files in branch having local commits
  - git diff master...  --name-status
  - git diff HEAD .
