## Committing changes I


 1. Make a change and commit (commit1)  
 
    <pre>
    <b>$ vi README.md</b>
    (Add a new line, eg. "Edit 1")
    <b>$ git status</b>  
    On branch master
    Your branch is up to date with 'origin/master'.

    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   README.md

    no changes added to commit (use "git add" and/or "git commit -a")

    <b>$ git add README.md</b>
    or
    <b>$ git add .</b>

    <b>$ git status</b>  
    On branch master
    Your branch is up to date with 'origin/master'.

    Changes to be committed:
      (use "git reset HEAD <file>..." to unstage)

        modified:   README.md
		
    <b>$ git commit</b>
    (enter message in editor)

    <b>$ git commit -m "First commit"</b>

    <b>$ gitk</b>

    </pre>
    
 
 2. Make a change and commit (commit2)

    <pre>
    <b>$ vi README.md</b>
    (Add a new line, eg. "Edit 2")
    
    <b>$ git status</b>
    
    <b>$ git add .</b>
    
    <b>$ git status</b>
    
    <b>$ git commit -m "Second commit"</b>
    
    <b>$ gitk</b>
    </pre>

 3. Make a change and commit (commit3)

    <pre>
    
    <b>$ vi README.md</b>
    (Add a new line, eg. "Edit 3")
    
    <b>$ git status</b>
    
    <b>$ git commit -a -m "Third commit"</b>
    
    <b>$ git status</b>
    
    <b>$ gitk</b>
    
    </pre>
    
 4. Refresh GitHub web
    
    Go to https://github.com/[GITHUB username]/git-training

    Eg. https://github.com/victorbarresf/git-training

    Check the last changes in README.md file are not visible yet  
      
        
 5. Push  

    <pre>
    <b>$ git push -u origin master</b>
    Enumerating objects: 11, done.
    Counting objects: 100% (11/11), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (6/6), done.
    Writing objects: 100% (9/9), 848 bytes | 121.00 KiB/s, done.
    Total 9 (delta 0), reused 0 (delta 0)
    To https://github.com/victorbarresf/git-training.git
    a553100..7f48b60  master -> master
    Branch 'master' set up to track remote branch 'master' from 'origin'.
    </pre>  
    
 6. Refresh GitHub web

    Go to https://github.com/[GITHUB username]/git-training

    Eg. https://github.com/victorbarresf/git-training

    Check the last changes in README.md file are already visible  


## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
