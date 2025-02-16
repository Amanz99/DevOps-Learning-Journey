# Basic Git Commands

## 1. git init
- Initializes a new Git repository in the current directory.

## 2. git clone <repository_url>
- Clones a remote repository to your local machine.
- Example: `git clone https://github.com/user/repo.git`

## 3. git status
- Displays the current state of the repository.
- Shows changes that have been staged, changes that are not staged, and files that aren't being tracked by Git.

## 4. git add <file>
- Adds files to the staging area before committing.
- Example: `git add index.html` to stage a single file, or `git add .` to stage all changes.

## 5. git commit -m "<message>"
- Commits the staged changes to the repository with a message.
- Example: `git commit -m "Fixed bug in the login feature"`

## 6. git push <remote> <branch>
- Pushes commits to a remote repository.
- Example: `git push origin main` to push to the `main` branch.

## 7. git pull <remote> <branch>
- Fetches changes from a remote repository and merges them into the local branch.
- Example: `git pull origin main` to pull changes from the `main` branch.

## 8. git branch
- Lists all the branches in the repository.
- `git branch <branch_name>` creates a new branch.

## 9. git checkout <branch_name>
- Switches to a different branch.
- Example: `git checkout feature-xyz`

## 10. git merge <branch_name>
- Merges changes from the specified branch into the current branch.
- A **merge conflict** occurs if changes in the merged branches are conflicting, meaning both branches have modified the same part of a file differently.
  
  ### How to avoid or fix a merge conflict:
  - **Avoid**: Communicate with your team to avoid working on the same parts of the code at the same time.
  - **Fix**: If a conflict occurs:
    1. Git will mark the conflict in the file with `<<<<<<<`, `=======`, and `>>>>>>>` markers.
    2. Open the file and decide which changes to keep.
    3. Remove the conflict markers and make necessary changes.
    4. Now use `git add <file>`.
    5. Commit the merge with `git commit`.

## 11. git log
- Displays the commit history for the repository.

## 12. git remote add <name> <url>
- Adds a new remote repository.
- Example: `git remote add origin https://github.com/user/repo.git`

## 13. git fetch
- Downloads new data from a remote repository but does not merge the changes automatically.
