## Stash changes

 1. Switch to **features/featureGFT**  
 
    <pre>
    <b>$ git checkout features/featureGFT</b>
    Switched to branch 'features/featureGFT'
    </pre>
    
 2. Create the file **Exercise7.txt** and move to stage area (do not commit it)  
 
    <pre>
    <b>$ vi Exercise7.txt</b>
    <b>$ git add .</b>
    </pre>
 3. Stash changes (right click on git repo)  

    <pre>
    <b>$ git stash</b>
    Saved working directory and index state WIP on features/featureGFT: 486d5fa Second change in feature branch
    </pre>
    
 4. Switch to **master** and commit 1 change  

    <pre>
    <b>$ git checkout master</b>
    Switched to branch 'master'
    Your branch is up to date with 'origin/master'.
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Change to check stash"</b>
    [master 4bed83d] Change to check stash
    1 file changed, 1 insertion(+)
    </pre>
    
 5. Back to **features/featureGFT**, recover the stash change and commit it.  
 
     <pre>
    <b>$ git checkout features/featureGFT</b>
    Switched to branch 'features/featureGFT'
    <b>$ git stash list</b>
    stash@{0}: WIP on features/featureGFT: 486d5fa Second change in feature branch
    <b>$ git stash apply</b>
    <b>$ git commit -m "Stash change committed"</b>
    [features/featureGFT 611c302] Stash change committed
    1 file changed, 1 insertion(+)
    create mode 100644 Exercise7.txt
    </pre>
     
 6. Push  

    <pre>
    <b>$ git push origin features/featureGFT</b>
    Enumerating objects: 4, done.
    Counting objects: 100% (4/4), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (2/2), done.
    Writing objects: 100% (3/3), 342 bytes | 114.00 KiB/s, done.
    Total 3 (delta 0), reused 0 (delta 0)
    To https://github.com/victorbarresf/git-training.git
    ba59e8f..611c302  features/featureGFT -> features/featureGFT
    </pre>

## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
