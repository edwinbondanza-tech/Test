# Test
Edwin's test repository
Common GitHub commands:
Here is a cheat sheet of common Git commands for local development, branching, and synchronizing with remote repositories. 
Setup and Initialization

These commands are used to configure Git for the first time and start a new project. 
git config --global user.name "[name]": Sets the username attached to your commits.
git config --global user.email "[email]": Sets the email address for your commits.
git init: Initializes a new local Git repository in the current directory.
git clone <url>: Downloads an existing project (repository) from a remote URL. 

Day-to-Day Work (Stage & Commit)
These are core commands for managing changes in your local repository. 
git status: Shows the status of your working directory, including new, modified, and untracked files.
git add <file>: Stages a specific file for the next commit.
git add .: Stages all changes and new files in the current directory and its subdirectories.
git commit -m "[message]": Records the staged snapshots permanently in the commit history with a descriptive message.
git diff: Shows unstaged changes between your working directory and the staging area.
git diff --staged: Shows changes between the staging area and the last commit. 

Branching and Merging
These commands manage different lines of development (branches). 
git branch: Lists all local branches.
git branch <branch-name>: Creates a new branch (but does not switch to it).
git checkout <branch-name>: Switches to the specified branch or commit. (The modern alternative is git switch <branch-name>).
git checkout -b <new-branch-name>: Creates a new branch and immediately switches to it.
git merge <branch-name>: Joins the specified branch's history into your current branch.
git branch -d <branch-name>: Deletes a local branch (only if it has been merged). Use -D to force deletion. 

Synchronizing with Remotes 
These commands interact with a shared remote repository (e.g., on GitHub or GitLab). 
git remote add origin <url>: Adds a remote repository to your local configuration.
git fetch: Downloads new data (commits, branches, tags) from the remote but doesn't integrate them into your working files.
git pull: Fetches changes from the remote and immediately merges them into your current branch. (This is a combination of git fetch and git merge).
git push origin <branch-name>: Uploads your local commits to the remote repository.
git push -u origin <branch-name>: Pushes the branch and sets it as the upstream, allowing you to use git push and git pull without arguments later. 

Undoing Changes
These commands help fix mistakes or discard local modifications. 
git restore <file> or git checkout -- <file>: Discards local changes to a specific file.
git reset --hard: Discards all staged and unstaged changes in the working directory and resets to the last commit. Use with caution.
git revert <commit-hash>: Creates a new commit that undoes the changes made in a specified previous commit, preserving project history.
git commit --amend: Modify the most recent commit message or add forgotten files to it (if not already pushed to a remote). 
For more in-depth learning, the official Pro Git book is available online for free, and visual cheat sheets are provided by GitLab and GitHub Education. 
