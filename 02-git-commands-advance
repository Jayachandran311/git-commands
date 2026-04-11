
# Git Commands (Advanced – Beyond Basics)

This document contains **commonly used Git commands** with **simple explanations and examples**.
Basic commands like `git init`, `git status`, `git add`, `git commit`, `git log`, `git diff`,
`git branch`, `git checkout`, `git merge`, `git clone`, `git pull`, and `git push` are intentionally excluded.

---

## Configure Git User – git config

Sets user information for commits.

```shell
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

---

## Rename or Move Files – git mv

Renames or moves files while keeping history.

```shell
git mv old.txt new.txt
```

---

## Remove Files – git rm

Deletes file and stages removal.

```shell
git rm test.txt
```

Remove from Git only:

```shell
git rm --cached config.yaml
```

---

## Restore Files – git restore

Discard local changes.

```shell
git restore app.js
```

Unstage file:

```shell
git restore --staged app.js
```

---

## Reset Commits – git reset

Moves HEAD to a previous commit.

```shell
git reset --soft HEAD~1
```

```shell
git reset --hard HEAD~1
```

---

## Revert Commit – git revert

Safely undo a commit by creating a new commit.

```shell
git revert <commit-id>
```

---

## Stash Changes – git stash

Temporarily save uncommitted changes.

```shell
git stash
git stash pop
```

---

## Manage Remotes – git remote

List remotes:

```shell
git remote -v
```

Add remote:

```shell
git remote add origin https://github.com/user/repo.git
```

---

## Fetch Changes – git fetch

Download remote changes without merging.

```shell
git fetch origin
```

---

## Rebase Branch – git rebase

Reapply commits on top of another branch.

```shell
git rebase main
```

---

## Cherry-pick Commit – git cherry-pick

Apply a specific commit from another branch.

```shell
git cherry-pick <commit-id>
```

---

## Tag Versions – git tag

Create a release tag.

```shell
git tag v1.0
git push origin v1.0
```

Annotated tag:

```shell
git tag -a v1.1 -m "Release 1.1"
```

---

## View Commit Details – git show

Displays details of a commit.

```shell
git show <commit-id>
```

---

## Track Line Changes – git blame

Shows who last changed each line.

```shell
git blame app.js
```

---

## Clean Untracked Files – git clean

Preview deletion:

```shell
git clean -n
```

Delete files:

```shell
git clean -f
```

---

## Summary

Useful commands for day‑to‑day Git usage beyond the basics.

**Tip:** Use these after you are comfortable with add, commit, pull, and push.
