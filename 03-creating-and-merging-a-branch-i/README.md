## Creating and merging a branch I



1.  Create and switch to a new branch **features/exercise3** 

    <pre>
    <b>$ git branch features/exercise3</b>
    features/exercise3 *master
    <b>$ git checkout features/exercise3</b>
    Switched to branch 'features/exercise3'
    </pre>
    
    or
    
    <pre>
    <b>$ git checkout -b features/exercise3</b>
    Switched to a new branch 'features/exercise3'
    </pre>
 
 

2.  Push the branch  
    
    <pre>
    <b>$ git push origin features/exercise3</b>
    Total 0 (delta 0), reused 0 (delta 0)
    remote:
    remote: Create a pull request for 'features/exercise3' on GitHub by visiting:
    remote:      https://github.com/victorbarresf/git-training/pull/new/features/exercise3
    remote:
    To https://github.com/victorbarresf/git-training.git
    [new branch]      features/exercise3 -> features/exercise3
    </pre>

 
3.  Commit a change  

   <pre>
   <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Added line in branch"</b>
    [features/exercise3 ba59e8f] Added line in branch
    1 file changed, 1 insertion(+)
   </pre>

 
4.  Merge changes to master  
    
4.1.  Switch to **master** branch  
    <pre>
            <b>$ git checkout master</b>
            Switched to branch 'master'
            Your branch is up to date with 'origin/master'.
    </pre>

4.2.  Merge from **features/exercise3** to **master**  
    <pre>
        <b>$ git merge features/exercise3</b>
        Updating fb5f3a8..ba59e8f
        Fast-forward
        README.md | 1 +
        1 file changed, 1 insertion(+)
    </pre>
    

5.  Push the changes  
    
    <pre>
    <b>$ git push -u origin master</b>
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 347 bytes | 115.00 KiB/s, done.
    Total 3 (delta 1), reused 0 (delta 0)
    remote: Resolving deltas: 100% (1/1), completed with 1 local object.
    To https://github.com/victorbarresf/git-training.git
    fb5f3a8..ba59e8f  master -> master
    Branch 'master' set up to track remote branch 'master' from 'origin'.
    </pre>


6.  Delete branch **features/exercise3**
 
   6.1.  Delete local branch   
    <pre>
        <b>$ git branch -D features/exercise3</b>
	     Deleted branch features/exercise3 (was ba59e8f).
    </pre>
   
   6.2.  Delete remote branch (remote – push) 
    <pre>
        <b>$ git push --delete origin features/exercise3</b>
	    To https://github.com/victorbarresf/git-training.git
	    -[deleted]         features/exercise3
    </pre>
        
 
7.  View GitHub  

    Go to https://github.com/[GITHUB username]/git-training

    Eg. https://github.com/victorbarresf/git-training


## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
