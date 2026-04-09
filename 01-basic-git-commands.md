# Basic Git Commands

This document explains **basic Git commands** in a **simple way**, with **small examples**, suitable for displaying in a portal or wiki.

---

## What is Git?

Git is a **version control system** used to track changes in code and collaborate with others.

---

## 1. Initialize a Repository – git init

Starts Git tracking in the current folder.

```Shell
git init
```

✅ Run once per project

---

## 2. Check Status – git status

Shows current state of files (modified, staged, untracked).

```Shell
git status
```

Think of it as: **"What is Git tracking right now?"**

---

## 3. Add Files – git add

Moves changes to the **staging area**.

Add one file:

```Shell
git add index.html
```

Add all files:

```Shell
git add .
```

---

## 4. Commit Changes – git commit

Saves a snapshot of staged changes.

```Shell
git commit -m "Initial commit"
```

✅ Always write a clear message

---

## 5. View Commit History – git log

Shows past commits.

```Shell
git log
```

---

## 6. View File Changes – git diff

Shows differences before commit.

```Shell
git diff
```

---

## 7. Create a Branch – git branch

Used to work on features safely.

Create branch:

```Shell
git branch feature-login
```

List branches:

```Shell
git branch
```

---

## 8. Switch Branch – git checkout

Moves to another branch.

```Shell
git checkout feature-login
```

---

## 9. Merge Branch – git merge

Combine one branch into another.

```Shell
git checkout main
git merge feature-login
```

---

## 10. Clone Repository – git clone

Creates a local copy of a remote repo.

```Shell
git clone https://github.com/user/repo.git
```

---

## 11. Pull Latest Changes – git pull

Fetches and merges changes from remote.

```Shell
git pull origin main
```

---

## 12. Push Changes – git push

Uploads commits to remote repository.

```Shell
git push origin main
```

---

## Common Daily Git Workflow

```Shell
git status
git add .
git commit -m "Your message"
git push
```

---

## Easy Memory Tip

**Check → Add → Commit → Push**

---

*End of document*