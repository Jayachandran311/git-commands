# Git Commands – Quick Guide with Examples

This document contains commonly used **Git commands**, their **purpose**, and **simple examples**.  
Useful for **learning, daily work, and interview preparation**.

---

## Repository Basics

### git init
Initializes a new Git repository in the current directory.
```bash
git init
```

### git clone
Creates a local copy of an existing remote repository.
```bash
git clone https://github.com/username/repo-name.git
```

---

## Status & Tracking

### git status
Shows the current state of files (modified, staged, untracked).
```bash
git status
```

---

## Adding Files to Staging Area

### git add <file>
Adds a specific file to staging.
```bash
git add one.txt
```

### git add .
Adds new and modified files (not deleted files).
```bash
git add .
```

### git add *
Adds files in the current directory only (no hidden files).
```bash
git add *
```

### git add --all / git add -A
Adds **new, modified, and deleted files** (recommended).
```bash
git add -A
```

---

## Reset (Undo)

### git reset
Unstages files but keeps changes.
```bash
git reset
```

### git reset HEAD~
Removes the last commit but keeps file changes.
```bash
git reset HEAD~
```

### git reset --hard
Deletes commits and changes permanently.
```bash
git reset --hard
```

---

## Removing Files

### git rm four.txt
Deletes file from both Git and local folder.
```bash
git rm four.txt
```

### git rm -f four.txt
Force delete a file even if modified.
```bash
git rm -f four.txt
```

### git rm --cached four.txt
Removes file from Git but keeps it locally.
```bash
git rm --cached four.txt
```

### git rm -r foldername
Deletes a folder and all its contents.
```bash
git rm -r foldername
```

---

## Commit History

### git log
Shows full commit history.
```bash
git log
```

### git log --oneline
Shows short commit history.
```bash
git log --oneline
```

---

## Branching

### git branch
Lists all local branches.
```bash
git branch
```

### git branch develop
Creates a branch from current branch.
```bash
git branch develop
```

### git checkout develop
Switches to develop branch.
```bash
git checkout develop
```

### git checkout <commit-id>
Moves to a specific commit.
```bash
git checkout d5gf81g5
```

---

## Merge & Diff

### git merge main
Merges main into current branch.
```bash
git merge main -m "merging"
```

### git diff
Shows unstaged changes.
```bash
git diff
```

### git diff <commit1> <commit2>
Compares two commits.
```bash
git diff abc26546 jdhfiahd
```

---

## Remote Commands

### git push origin main
Push main branch to remote.
```bash
git push origin main
```

### git push
Push current branch.
```bash
git push
```

### git fetch
Downloads changes without merge.
```bash
git fetch
```

### git merge
Merges fetched changes.
```bash
git merge
```

### git pull
Fetch + merge.
```bash
git pull
```

---

## Restore

### git restore one.txt
Undo file changes.
```bash
git restore one.txt
```

### git restore foldername
Undo folder changes.
```bash
git restore foldername
```

### git restore .
Undo all unstaged changes.
```bash
git restore .
```

---

## Stash

### git stash
Save work temporarily.
```bash
git stash
```

### git stash list
List stashes.
```bash
git stash list
```

### git stash apply
Apply stash (keep it).
```bash
git stash apply
```

### git stash pop
Apply and delete stash.
```bash
git stash pop
```

### git stash drop
Delete stash.
```bash
git stash drop
```
