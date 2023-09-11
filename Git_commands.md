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
   
   P.S.: uncomitted, unstaged (file known before), untracked files (i.e. completely new file)

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
9. How to bring changes from the remote to the local repository?
   - 'git pull'
   observation: when your local is not synced with the remote (e.g. when collaborating or when changing something online?)
