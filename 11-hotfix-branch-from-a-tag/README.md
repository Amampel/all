## Hotfix branch from a tag

 1. Create the branch **hotfixes/hotfix1** from tag **Release1.0**  
  
    <pre>
    <b>$ git checkout -b hotfixes/hotfix1 v1.0</b>
    Switched to a new branch 'hotfixes/hotfix1'
    </pre>

 2. Fix the issue  

    <pre>
    <b>$ vi README.md</b>
    </pre>  
    
 3. Commit & push  

    <pre>
    <b>$ git add .</b>
    <b>$ git commit -m "Fixed issue in hotfix branch"</b>
    [hotfixes/hotfix1 22acffd] Fixed issue in hotfix branch
    1 file changed, 14 insertions(+), 13 deletions(-)
    rewrite README.md (66%)
    <b>$ git push -u origin hotfixes/hotfix1</b>
    Enumerating objects: 5, done.
    Counting objects: 100% (5/5), done.
    Delta compression using up to 4 threads
    Compressing objects: 100% (3/3), done.
    Writing objects: 100% (3/3), 408 bytes | 136.00 KiB/s, done.
    Total 3 (delta 2), reused 0 (delta 0)
    remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
    remote:
    remote: Create a pull request for 'hotfixes/hotfix1' on GitHub by visiting:
    remote:      https://github.com/victorbarresf/git-training/pull/new/hotfixes/hotfix1
    remote:
    To https://github.com/victorbarresf/git-training.git
    *[new branch]      hotfixes/hotfix1 -> hotfixes/hotfix1
    Branch 'hotfixes/hotfix1' set up to track remote branch 'hotfixes/hotfix1' from 'origin'.
    </pre>

 4. Switch to master and merge **hotfixes/hotfix1**  

    <pre>
    <b>$ git checkout master</b>
    Switched to branch 'master'
    Your branch is ahead of 'origin/master' by 1 commit.
    (use "git push" to publish your local commits)
    <b>$ git merge hotfixes/hotfix1</b>
    </pre>
    
 5. Delete local & remote **hotfixes/hotfix1** branch  
 
    <pre>
    <b>$ git branch -d hotfixes/hotfix1</b>
    Deleted branch hotfixes/hotfix1 (was 9b8f855).
    <b>$ git push --delete origin hotfixes/hotfix1</b>
    To https://github.com/victorbarresf/git-training.git
    -[deleted]         hotfixes/hotfix1
    </pre>
 
## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
