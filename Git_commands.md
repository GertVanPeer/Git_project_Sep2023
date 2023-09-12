# Manual of Git commands

1. How to initialize git?
   
   `git init`

2. How to send to staging area?
   
   `git add <file name>`
   
   **How to use it cleverly?**
   
   - use in combination with git status 
   
   - `git add` files with related changes
   
   - `git commit` with message

3. How to commit a change to create my 1st snapshot?
   
   `git commit -m "MEANINGFUL MESSAGE"`
   
   P.S.: Meaningful message: why, how, limitations, effects

4. How to check in what conceptual areas my files are?
   
   `git status`
   
   P.S.: uncommitted, unstaged (file known before), untracked files (i.e. completely new file)

5. How to get commit history?
   
   `git log`
   
   interesting arguments:
   
   - `-n`
   
   - `--abbrev-comit`
   
   - `git log` `optional/path/to/specific/file`

6. How to compare versions of the same file?
   
   - `git show `<commit 1> <commit 2>  (or you can specify a single commit and you'll get the difference with the previous commit)
   
   - `git diff` <commit 1> <commit 2>
   
   Take into account the directionality!

7. How to establish the connection ('bridge') between your local git repository and the remote repository?
   
   - create a new repository online; it's easiest to use the same name as your local repository
   
   - creating the link: use the command `git remote add` <name for connection> <SSH key>
     
     - name for link: usually you used the same as for both repositories, but it can be anything basically
   
   - SSH key is different for each repository and can be retrieved in GitHub

8. How to transfer your commits to your remote repository on GitHub?
   
   - `git push`

9. How to get rid of a commit?
   
   - `git revert HEAD`: will revert you to the previous commit (i.e. changes HEAD to the previous commit)
     
     (**<u>best not to use</u>** `git reset` as long as you don't know what you're doing)

10. How to recover your local repository when you accidentally delete it?
    
    - `git clone <SSH key>`



#### Collaborations

1. How to start a new collaboration?
   
   To start a new collaboration you have to go to your GitHub repository and give access to your collaborator.
   
   Go to **Settings** -> **Collaborators** (Access section on the left sidebar) -> green button **Add people** -> Add email/username/full name of the potential collaborator.
   
   Your collaborator should accept the invitation. From now on he/she will have access to push/pull your project.

2.  How to make the corresponding repository to your computer?
   
   To start working on your collaborative project you should make a new folder on your computer (**<u>DO NOT ADD NEW GIT CONTROLLED PROJECT INSIDE ANOTHER FOLDER WITH INITIATED GIT</u>**).
   
   Go to this folder using `cd` and `git clone <ssh>` for the collaborative project. This will already make the bridge and grant you access to push/pull to the project.
