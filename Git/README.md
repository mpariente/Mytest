## Git Tutorial :

Steps taken from [this tutorial](https://github.com/GarageGames/Torque2D/wiki/Cloning-the-repo-and-working-with-Git)

1. **Fork** the repo into your account
2. **Clone** your fork using `git clone URL_fork path/to/folder`
3. Set up a **remote** to the original repo :
  * `git remote add remote_name URL_original_repo`
  * Check remotes with `git remote -v`
    * The remote `origin` corresponds to your fork
    * The remote `remote_name` corresponds to the original repo
4. Manage **branches**
  * **List** branches with `git branch`
  * **Create** new branch with `git branch branch_name`
  * **Switch** to branch woth `git checkout branch_name`
5. Good practice is :
  ```
  git branch new_branch
  git checkout new_branch
  git pull remote_name target_branch
  ```  
  This creates a new branch, makes it the currently active branch  
  and pull the contents of the target branch from the original repo  
  into our currently active branch (**Be sure to `chechout` the good one !**)

6. Make your changes
7. Update your online repo
  * `git add .` or `git add filename1 filename2`  
  You can run `git status` to check what's happening
  * `git commit -m 'Message about the commit'`
  * `git push remote_name branch_name` , here :  
   `git push origin new_branch`
