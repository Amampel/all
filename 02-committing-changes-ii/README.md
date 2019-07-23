## Committing changes II

 1. Make a change and commit (commit1)  
  
    <pre>
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Added line"</b>
    </pre>
 2. Make a change and commit (commit2)  
    <pre>
    <b>$ vi README.md</b>
    <b>$ git add .</b>
    <b>$ git commit -m "Added new line"</b>
    <b>$ git log</b>
    </pre>
 3. Combine all changes in a single commit (reset)  
    <pre>
    <b>$ git reset --soft HEAD~2</b>
    <b>$ git log</b>     (notice the last 2 commits have left)
    <b>$ git commit -m "Commit after reset"</b>
    <b>$ git log</b>
    </pre>
 4. Push  
    <pre>
    <b>$ git push -u origin master</b>
    </pre>

## License
Copyright (C) 2017 GFT. All rights reserved.

## Author Information
* Agile & Devops Practice Iberia. GFTIberia.PSU_Technology@gft.com
