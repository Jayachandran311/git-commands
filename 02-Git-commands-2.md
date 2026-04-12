# Git Basics Cheat Sheet

## git revert

- Used to undo a commit safely by creating a new commit
- Does not rewrite history
- Safe for shared branches

```bash
git revert <commit-hash>
```

---

## git reset vs git revert

### git reset

- Moves HEAD backward
- Rewrites history
- Use only for local commits

```bash
git reset --soft HEAD~1   # keeps changes staged
git reset --mixed HEAD~1  # keeps changes unstaged (default)
git reset --hard HEAD~1   # discards changes (dangerous)
```

### git revert

- Creates a new commit that cancels a previous commit
- Safe for public/shared branches

---

## git rebase

- Reapplies commits on top of another branch
- Creates linear commit history
- Rewrites history

```bash
git rebase <base-branch>
```

---

## git rebase main

- Replays current branch commits on top of `main`

```bash
git checkout feature
git rebase main
```

---

## Pull Request vs Merge Request

- GitHub: Pull Request (PR)
- GitLab: Merge Request (MR)
- Same concept, different names
- Used for code review and merging changes
