# Test Project 1
# My Project
# My Project from Terminal 



Great — you're ready to **take full control over GitHub from the terminal**. Here's a cheat sheet-style guide to everything you need — no GitHub website needed unless you want to view things visually.

---

## ✅ 1. Clone Any Repo (SSH)

```bash
git clone git@github.com:username/repo.git
cd repo
```

---

## ✅ 2. Create a New Local Repo and Push It to GitHub

1. Create the repo on GitHub **(only once)** using the site
2. Then in terminal:

```bash
mkdir myproject
cd myproject
git init
touch README.md
git add .
git commit -m "First commit"
git branch -M main
git remote add origin git@github.com:username/myproject.git
git push -u origin main
```

---

## ✅ 3. Common Daily Git Commands

### Make changes and push:

```bash
git add .
git commit -m "your message"
git push
```

### Pull latest changes from GitHub:

```bash
git pull
```

---

## ✅ 4. Check Status and History

```bash
git status         # See changed/uncommitted files
git log --oneline  # See commit history in short form
```

---

## ✅ 5. Create and Use Branches

```bash
git checkout -b new-branch     # Create and switch to a branch
git checkout main              # Switch back to main
git merge new-branch           # Merge into current branch
git branch -d new-branch       # Delete branch locally
git push origin new-branch     # Push branch to GitHub
```

---

## ✅ 6. Set Remote If You Forgot

```bash
git remote add origin git@github.com:username/repo.git
```

See current remote:

```bash
git remote -v
```

---

## ✅ 7. Rename the Remote (Optional)

```bash
git remote rename origin github
```

---

## ✅ 8. SSH Key Already Set (you did this!)

You're using:

```bash
git@github.com:...
```

So you're all good — no password needed for pushes.

---

## ✅ 9. Delete Repo from GitHub (via GitHub CLI)

Optional advanced setup:

Install GitHub CLI:

```bash
brew install gh
```

Login:

```bash
gh auth login
```

Then you can delete or create repos from terminal:

```bash
gh repo create my-repo --public
gh repo delete username/repo-name --confirm
```

---

## ✅ 10. Backup All Projects from Terminal (optional)

You can even write a script to pull/push all your local projects. Let me know if you'd like that.

---

You're now 100% ready to manage your GitHub workflow directly from the terminal.

Would you like me to generate a `.gitignore`, README template, or setup automation (like `pre-commit` or hooks)?

