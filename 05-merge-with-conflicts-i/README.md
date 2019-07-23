## Merge with conflicts I

1. Switch to **master**  

     <pre>
     <b>$ git checkout master</b>
        Switched to branch 'master'
        Your branch is up to date with 'origin/master'.
     </pre>
 
2. Commit 2 changes  

    <pre>
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "First change in master branch"</b>
    [master 1c70a90] First change in master branch
    1 file changed, 1 insertion(+)
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Second change in master branch"</b>
    [master 17bbc25] Second change in master branch
    1 file changed, 1 insertion(+)
    </pre>
    
3. Switch to **features/featureGFT**  
 
    <pre>
    <b>$ git checkout features/featureGFT</b>
    Switched to branch 'features/featureGFT'
    </pre>

4. Commit 2 changes

    <pre>
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "First change in feature branch"</b>
    [features/featureGFT 9621c56] First change in feature branch
    1 file changed, 1 insertion(+)
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Second change in feature branch"</b>
    [features/featureGFT 486d5fa] Second change in feature branch
    1 file changed, 1 insertion(+)
    </pre>
    
5. View history view  
 
    <pre>
    <b>$ git log --all</b>
    </pre>

6. Switch to **master** and merge **features/featureGFT**  
 
    <pre>
    <b>$ git checkout master</b>
    Switched to branch 'master'
    Your branch is ahead of 'origin/master' by 2 commits.
    (use "git push" to publish your local commits)
    <b>$ git merge features/featureGFT</b>
    Auto-merging README.md
    CONFLICT (content): Merge conflict in README.md
    Automatic merge failed; fix conflicts and then commit the result.
    </pre>

7. Resolve the conflicts and commit  
    <pre>
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "After solving conflicts"</b>
    [master 4559aba] After solving conflicts
    <b>$ git log</b>
    </pre>

## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
