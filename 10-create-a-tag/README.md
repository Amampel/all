## Create a tag

 1. Switch to master  

    <pre>
    <b>$ git checkout master</b>
    Switched to branch 'master'
    Your branch is up to date with 'origin/master'.
    </pre>
    
 2. Create and push the tag **Release1.0**  
 
    <pre>
    <b>$ git tag</b>
    <b>$ git tag -a v1.0 -m ""</b>
    </pre>  

 3. Commit and push a change  

    <pre>
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Test tag command"</b>
    [master 6db0994] Test tag command
    1 file changed, 1 insertion(+)
    <b>$ git push origin v1.0</b>
    Enumerating objects: 1, done.
    Counting objects: 100% (1/1), done.
    Writing objects: 100% (1/1), 153 bytes | 51.00 KiB/s, done.
    Total 1 (delta 0), reused 0 (delta 0)
    To https://github.com/victorbarresf/git-training.git
    *[new tag]         v1.0 -> v1.0
    <b>$ git tag</b>
    v1.0
    <b>$ git show v1.0</b>
    tag v1.0
    Tagger: VRBS <victor.barres@gft.com>
    Date:   Tue Nov 13 09:06:45 2018 +0100
    commit 6cb47c442d0b90952748b797814b486d38663093 (tag: v1.0, origin/master, origin/HEAD)
    Author: victorbarresf <44898471+victorbarresf@users.noreply.github.com>
    Date:   Mon Nov 12 18:20:02 2018 +0100
    </pre>
    

## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
