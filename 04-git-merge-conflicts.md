# GitHub / GitLab Merge Conflicts

## What Is a Merge Conflict?
A **merge conflict** occurs when Git cannot automatically merge changes from two branches because the **same file and same lines** were modified differently.

GitHub and GitLab both use **Git**, so merge conflicts behave the same on both platforms.

---

## Common Causes
- Two contributors edited the **same lines** in a file
- One branch **deleted** a file while another **modified** it
- Long-running branches not frequently updated with the main branch

---

## How a Merge Conflict Looks
```text
<<<<<<< HEAD
code from current branch
=======
code from branch being merged
>>>>>>> feature-branch
```

---

## How to Resolve a Merge Conflict (CLI)

### 1. Start the merge
```bash
git checkout main
git merge feature-branch
```

### 2. Identify conflicted files
```bash
git status
```

### 3. Edit conflicted files
- Open the file
- Decide which changes to keep or merge
- Remove all conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)

### 4. Mark conflict as resolved
```bash
git add <file>
```

### 5. Complete the merge
```bash
git commit
```

---

## Resolving Conflicts in GitHub / GitLab UI
1. Open the Pull Request / Merge Request
2. Click **Resolve conflicts**
3. Edit the file in the browser
4. Remove conflict markers
5. Mark as resolved
6. Commit and merge

---

## Best Practices to Avoid Conflicts
- Pull latest changes frequently
```bash
git pull origin main
```
- Keep feature branches short-lived
- Avoid parallel edits on the same lines
- Rebase feature branches regularly
```bash
git rebase main
```

---

## Summary
- Merge conflicts occur when Git cannot auto-merge
- Manual resolution is required
- Same behavior in GitHub and GitLab
- Proper branching strategy reduces conflicts
