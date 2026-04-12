# Advanced Git Commands – Explanation & Examples

This document covers **important Git commands** often missing from basic guides.
Each command includes a **clear explanation** and a **practical example**.

---

## Branching (Modern Commands)

### git switch
Switch between branches (recommended replacement for `git checkout`).
```bash
git switch main
```

### git switch -c <branch>
Create and switch to a new branch.
```bash
git switch -c feature/login
```

### git restore --staged <file>
Unstage a staged file without losing changes.
```bash
git restore --staged app.js
```

---

## Rebase – Advanced

### git rebase -i
Interactive rebase to edit, squash, or reorder commits.
```bash
git rebase -i HEAD~3
```

### git rebase --continue
Continue rebase after resolving conflicts.
```bash
git rebase --continue
```

### git rebase --abort
Cancel the rebase and return to previous state.
```bash
git rebase --abort
```

### git rebase --skip
Skip the commit causing conflict.
```bash
git rebase --skip
```

---

## Cherry-pick

### git cherry-pick <commit>
Apply a specific commit from another branch.
```bash
git cherry-pick a1b2c3d
```

### git cherry-pick --abort
Cancel cherry-pick after conflict.
```bash
git cherry-pick --abort
```

### git cherry-pick --continue
Continue cherry-pick after resolving conflict.
```bash
git cherry-pick --continue
```

---

## Revert – Advanced

### git revert HEAD
Revert the latest commit safely.
```bash
git revert HEAD
```

### git revert --no-commit <commit>
Prepare revert without auto commit.
```bash
git revert --no-commit a1b2c3d
```

---

## Reset – Modes

### git reset --soft
Undo commit, keep changes staged.
```bash
git reset --soft HEAD~1
```

### git reset --mixed
Undo commit, keep changes unstaged (default).
```bash
git reset --mixed HEAD~1
```

### git reset --hard
Undo commit and delete all changes (dangerous).
```bash
git reset --hard HEAD~1
```

---

## Tags

### git tag
List all tags.
```bash
git tag
```

### git tag -a <tag>
Create annotated tag.
```bash
git tag -a v1.0 -m "Release version 1.0"
```

### git push origin --tags
Push tags to remote.
```bash
git push origin --tags
```

---

## Remote Management

### git remote -v
View remote URLs.
```bash
git remote -v
```

### git remote add
Add a new remote.
```bash
git remote add upstream https://github.com/org/repo.git
```

### git remote remove
Remove a remote.
```bash
git remote remove upstream
```

### git remote rename
Rename a remote.
```bash
git remote rename origin old-origin
```

---

## Fetch & Pull (Advanced)

### git fetch origin <branch>
Fetch specific branch without merging.
```bash
git fetch origin develop
```

### git pull --rebase
Pull changes using rebase instead of merge.
```bash
git pull --rebase origin main
```

---

## Log & History

### git log --graph
Graphical commit history.
```bash
git log --graph --oneline --all
```

### git log --decorate
Show branches and tags in log.
```bash
git log --decorate
```

### git show
View details of a commit.
```bash
git show a1b2c3d
```

---

## Debugging

### git blame
See who changed each line.
```bash
git blame app.js
```

### git bisect
Find commit that introduced a bug.
```bash
git bisect start
git bisect bad
git bisect good v1.0
```

---

## Cleaning Working Directory

### git clean -n
Preview untracked file deletion.
```bash
git clean -n
```

### git clean -f
Delete untracked files.
```bash
git clean -f
```

---

## Configuration

### git config --global user.name
Set username.
```bash
git config --global user.name "Your Name"
```

### git config --global user.email
Set email.
```bash
git config --global user.email "you@email.com"
```

### git config --list
View all configuration.
```bash
git config --list
```

---

## Ignore Files

### .gitignore
Ignore files from tracking.
```text
node_modules/
.env
*.log
```

### git check-ignore
Check why file is ignored.
```bash
git check-ignore -v file.txt
```

---

## Recovery

### git reflog
Recover lost commits or resets.
```bash
git reflog
```

---

✅ **Recommended for Interviews & Production Work**
