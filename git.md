# Git Cheat Sheet

## Core Terms/Concepts

- **Repository (Repo)**: A Git-tracked project containing a `.git` directory that stores the entire version history, metadata, branches, and configuration.
- **Working Directory**: The actual files on your filesystem that you modify. 
- **Staging Area (Index)**: A temporary area where changes are prepared before committing.
- **Commit**: A saved snapshot of staged changes.
- **HEAD**: Pointer to the current commit.
- **Branch**: A movable pointer to a commit; allows parallel development.
- **Main (or Master)**: The default primary branch.
- **Merge**: Combines changes from one branch into another.
- **Merge**: Conflict When Git can’t automatically merge changes.
- **Rebase**: Reapplies commits on top of another branch to create a cleaner history.
- **Remote**: A version of your repo hosted online (e.g., GitHub).
- **Origin**: Default name for the main remote repository.
- **Clone**: copies a remote repository to your machine.
- **Pull**: Fetches and merges changes from a remote branch.
- **Push**: Uploads your local commits to the remote repository.
- **Fetch**: Downloads remote changes without merging.
- **Pull Request (PR)**: A request to merge changes (GitHub feature).
- **Fork**: A personal copy of someone else’s repository.

## Commands

### Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list
```

---

### Starting a Repository

```bash
git init                 # Initialize new repo
git clone <repo-url>     # Clone existing repo
```

### Basic Workflow

```bash
git status               # Check status
git add <file>           # Stage file
git add .                # Stage all changes
git commit -m "message"  # Commit
git log
```

### Branching

```bash
git branch
git branch <name>
git checkout <name>
git checkout -b <name>
git switch <name>
git merge <branch>
git branch -d <name>
```

---

### Remote Repositories

```bash
git remote -v
git remote add origin <url>
git push -u origin main
git pull
git fetch
```

---

### Undoing Changes

```bash
git restore <file>
git restore --staged <file>
git reset --soft HEAD~1
git reset --hard HEAD~1
git revert <commit-hash>
```

---

### Stashing

```bash
git stash
git stash list
git stash pop
git stash apply
```

---

### Inspecting Changes

```bash
git diff
git diff --staged
git show <commit-hash>
```

---

### Tags

```bash
git tag
git tag v1.0.0
git push origin v1.0.0
```

---

### Helpful Pro Tips

```bash
git log --oneline --graph --all
git commit --amend
git rebase main
git clean -fd
```
