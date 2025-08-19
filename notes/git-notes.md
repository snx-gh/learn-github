
Learning Git - notes
============================
* SCM, version control, git-scm.com 
* git config —global user.name “snx”
* git config --global user.email “saurabhcnigam@users.noreply.github.com”
* Initialize your project for use with git & github
    * git init
* Add all untracked files to staging
    * git add .
* Commit the changes done so far, a checkpoint to come back to
    * git commit -m “first commit”
* Check logs for commit history
    * git log
    * git log --oneline  
* RESTORE: If tracked files are modified but not in staging and changes not required, restore it
    * git restore .
    * git restore README.md
* RESTORE: If changes are in staging but changes not required, restore it
    * git restore —staged README.md
* If files are not tracked, but changes are not required, delete the file/changes manually.
* GITIGNORE- sensitive files, personal notes, system files etc.
    * touch .gitignore && vi .gitignore
    * .DS_Store
    * .vscode/
    * node_modules
    * Global ignore file: git config —global core.excludesfile [file]
    * Clean dirty cache (may require new commit) : git rm -r —cached .
* remove and rename a file and add  to staging
    * git rm file.txt
    * git mv file.txt new.txt
* difference in tracked modified files 
    * git diff
* MODIFY COMMIT
    * git commit —amend
* RESET COMMIT, changes are not removed
    * git reset <commit to point HEAD to>
    * to lose the changes: git reset —hard <commit to point HEAD to>
* REBASE to move the commit in commit order with changes
    * git rebase -i —root
    * when editing the rebase 
        * we can move commit order
        * squash - use commit, but meld into previous commit
        * fixup - like squash but does not keep commit message
* BRANCHES (git flow)
    * git branch
    * new feature/fix branch: git switch -c newb or git checkout -b newb
    * make changes in new branch
    * merge to main/master: git switch main && git merge newb
    * delete old branch: git branch —d newb (ignores conflict)
* MERGE CONFLICT
    * VS code extension: Live server
    * if main/master was changed after checkout to new branch, conflict would occur while merging new branch to master
    * we can accept incoming change or reject it, and manually fix the conflict code
* STASH
    * put away code temporarily, stash is a stack
    * git stash [list | apply | pop]
* CLEAN
    * git clean -n #dry run only files
    * git clean -d #includes directory in dry run
    * git clean -f #force






