# Publishing a Local Repository to Remote
  1. Create local changes and commit them
  2. Create a remote repository on Github and add it to the local repo
     ```bash
      git remote add origin <remote_origin_url>
      ```
  3. Move the main  branch to main if it is not already main.
      ```
      git branch -M main 
      ```

  4. Push the branch to remote and set it to track the remote branch 
     ```
       git push -u origin main | git push --set-upstream origin main
     ```
     
  ## Creating  pull Requests
    1. Create the new branch for the feature and commit it to the the repository you forked in your account
      ```git
       git checkout -b <feature_branch>

       git push -u origin  <feature_branch>
      ```
    2. After committing the feature branch, a new pull request appears. You can now compare the differences between the the two branches, in this case the PULL-REQUESTS branch and the main branch of the repository you forked from. It uses the git diff command to compare the two branches. It shows  files have been added, removed, deleted, changed and so on.
      ```git

         git diff main PUll-REQUESTS 
         
      ````
      