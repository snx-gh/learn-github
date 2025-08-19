Learning GITHUB - notes
=======================

* Github cli:
    * Install gh CLI    brew install gh
    * Login:         gh auth login
    * Create repo:   gh repo create --public learn-github
    * Delete repo:   gh repo delete <repo>
    * List repo:     gh repo list

* REMOTE
    * git remote add <name> <url>
    * git rename OLDNAME NEWNAME
    * git remote -v
    * git remote add origin <url>
    - Ex: git remote add origin https://github.com/snx-gh/learn-github.git 
    
* PUSH
    * git push -u <remote-name> <branch-to-push>  # -u option sets upstream 
    * git push --all                              # push all branches
    * git branch -u <origin/remote-branch>        # to specify remote branch 
    * git push -u origin main 
    - Ex: git push --all 


* Github Flow
    * Main branch
    * Checkout to Feature branch
    * Commit and push to feature branch
    * Create pull requests
        * Ask for merge
        * Review requests
        * Feedbacks
    * Merge Pull requests
        * Merge process
        * Review conflicts
        * delete feature branch


* Markdown
    * # headline level 1
    * == headline level 1
    * -- sub-headline
    * __bold__ or **bold**
    * _italic_ or *italic*
    * ~~strikethrough~~
    * > Quotation
    * --- horizontal rule
    * *** Astericks
    * ___ Underscores


