# Git Commands  

---

## 🔹 Cherry Pick  
- `git cherry-pick "Commit ID"` → Copies a specific commit from another branch to the current branch  

---

## 🔹 Conflicts  
- Conflicts occur when two branches change the **same part of a file** and Git cannot automatically merge them.  
- Git marks the conflicting areas in the file, and you must **manually resolve** them.  
- After fixing, mark as resolved and commit:  
  ```bash
  git add "File"
  git commit

  # Git Commands  

---

## 🔹 Hotfixes  
- A **hotfix** is an urgent fix applied directly to production to resolve a **critical bug**.  
- Workflow:  
  ```bash
  git checkout main
  git checkout -b hotfix-branch
  # make the fix
  git commit -m "Fix: urgent issue"
  git checkout main
  git merge hotfix-branch
  git push origin main

