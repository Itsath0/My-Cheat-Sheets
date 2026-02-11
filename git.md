# Git Cheat Sheet

## Core Terms/Concepts

- **Repository (Repo)** A Git-tracked project containing a `.git` directory that stores the entire version history, metadata, branches, and configuration.
- **Working Directory** The actual files on your filesystem that you modify. 
- **Staging Area (Index)** A temporary area where changes are prepared before committing.
- **Commit** A saved snapshot of staged changes.
- **HEAD** Pointer to the current commit.
- **Branch** A movable pointer to a commit; allows parallel development.
- **Main (or Master)** The default primary branch.
- **Merge** Combines changes from one branch into another.
- **Merge** Conflict When Git can’t automatically merge changes.
- **Rebase** Reapplies commits on top of another branch to create a cleaner history.
- **Remote** A version of your repo hosted online (e.g., GitHub).
- **Origin** Default name for the main remote repository.
- **Clone** Copies a remote repository to your machine.
- **Pull** Fetches and merges changes from a remote branch.
- **Push** Uploads your local commits to the remote repository.
- **Fetch** Downloads remote changes without merging.
- **Pull Request (PR)** A request to merge changes (GitHub feature).
- **Fork** A personal copy of someone else’s repository.

### Commands

`git clone <url for your repo>` Clones A Repo (Remote/Local) to your filesystem

`git status` ??

`git add <file path>` Adds to the staging area 
note: you can add all files by using * in the file path argument

`git reset HEAD <file path>` Removes from the staging area

`git commit -m <Discription>` Adds to the local Repo

