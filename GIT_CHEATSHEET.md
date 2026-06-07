# Git Cheatsheet (Real Cases)

Short guide for daily work in this repository.

## 1) Check status before doing anything

```bash
git status -sb
git branch
git fetch origin
```

## 2) Safe flow to merge your work into main

```bash
git checkout main
git pull origin main
git merge your-branch
git push origin main
```

If there are conflicts:

```bash
# edit files
git add .
git commit
git push origin main
```

## 3) Save local changes quickly (including untracked files)

```bash
git stash push -u -m "temp work"
```

Bring changes back:

```bash
git stash pop
```

See stash list:

```bash
git stash list
```

## 4) Fix error: "untracked files would be overwritten"

This means a local file blocks checkout/merge.

Option A (keep your file):

```bash
move blocked_file.txt blocked_file_backup.txt
```

Option B (remove local file):

```bash
rm blocked_file.txt
```

Then retry merge/checkout.

## 5) Windows locked file ("file is being used by another process")

Close notebook/kernel or Python process, then retry.

PowerShell:

```powershell
Get-Process python, jupyter, ipykernel -ErrorAction SilentlyContinue
Get-Process python -ErrorAction SilentlyContinue | Stop-Process -Force
Remove-Item .\log.txt -Force
```

## 6) Ignore files that should not be committed

In `.gitignore`:

```gitignore
README_example.md
log.txt
```

If file was already tracked before:

```bash
git rm --cached log.txt
git commit -m "Stop tracking log file"
git push
```

## 7) Verify local repo is exactly like GitHub

```bash
git fetch origin
git rev-parse HEAD
git rev-parse origin/main
```

If hashes are different, pull main:

```bash
git pull --ff-only origin main
```
