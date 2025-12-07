# Git Commands to Add Portfolio to Repository

## Step 1: Navigate to the portfolio directory
```bash
cd C:\Users\emaho\knowledge-base-portfolio
```

## Step 2: Initialize Git repository (if not already initialized)
```bash
git init
```

## Step 3: Add all files to staging
```bash
git add .
```

## Step 4: Create initial commit
```bash
git commit -m "Initial commit: Knowledge Base Writer Portfolio"
```

## Step 5: Add remote repository (replace with your repository URL)
```bash
git remote add origin https://github.com/yourusername/your-repo-name.git
```

## Step 6: Rename branch to main (if needed)
```bash
git branch -M main
```

## Step 7: Push to remote repository
```bash
git push -u origin main
```

---

## Alternative: If you already have a remote repository

If your repository already exists and has files, you might need to pull first:

```bash
# Pull existing files (if any)
git pull origin main --allow-unrelated-histories

# Then push your changes
git push -u origin main
```

---

## If you get authentication errors:

You may need to authenticate. Options:
1. Use GitHub CLI: `gh auth login`
2. Use personal access token instead of password
3. Use SSH instead of HTTPS: `git remote set-url origin git@github.com:yourusername/your-repo-name.git`

---

## Quick one-liner (after initial setup):
```bash
git add . && git commit -m "Update portfolio" && git push
```

