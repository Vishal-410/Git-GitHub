# 🚀 Git Notes

A concise reference for **Git commands** and **SSH setup**.  
Perfect for quick revision during development.

---

## 📌 Git Basics
- `git init` → Initialize repo  
- `git add .` → Stage all changes  
- `git commit -m "message"` → Commit staged changes  
- `git status` → Show file status  
- `git log --oneline` → View commit history (compact)  

---

## 🌿 Branching
- `git branch feature` → Create branch  
- `git switch feature` → Switch branch  
- `git merge feature` → Merge branch into current  
- `git branch -d feature` → Delete branch  

---

## 🔄 Undo / Reset
- `git reset --soft HEAD~1` → Undo commit (keep staged)  
- `git reset --mixed HEAD~1` → Undo commit (keep unstaged)  
- `git reset --hard HEAD~1` → Undo + delete changes  
- `git revert <hash>` → Safe undo (creates new commit)  

---

## 📦 Remote Repos
- `git remote add origin <url>` → Add remote  
- `git push -u origin main` → Push branch  
- `git pull` → Fetch + merge  
- `git fetch` → Fetch only  
- `git branch -r` → List remote branches  

---

## 🕒 Stash
- `git stash` → Save changes temporarily  
- `git stash list` → List stashes  
- `git stash apply stash@{0}` → Apply stash  
- `git stash pop` → Apply + remove stash  

---

## 🔑 SSH Setup
- `ssh-keygen -t ed25519 -C "youremail@example.com"` → Generate key  
- `ssh-add ~/.ssh/id_ed25519` → Add private key  
- `ssh -T git@github.com` → Test connection  

---

## ✅ Best Practices
- Always **pull before push**  
- Use **branches** for new features  
- Prefer `git revert` over `reset --hard` on shared repos  
- Add a **.gitignore** to avoid committing unwanted files  

---

## 📊 Visual Git Workflow
