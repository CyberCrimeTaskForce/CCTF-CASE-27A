# GIT & GITHUB INVESTIGATOR CHEAT SHEET
**REFERENCE:** CCTF-TECH-01  
**PURPOSE:** QUICK-REFERENCE GUIDE FOR REPOSITORY FORENSICS  

---

### 1. GITHUB WEB INTERFACE NAVIGATION

* **Commit History:** Click the commit count (e.g., `12 commits`) to view the chronological log of changes. Click any commit hash to inspect the **Diff** (green lines = added text; red lines = deleted text).
* **Branch Selector:** Use the branch dropdown (top-left of file tree) to switch between `main` and secondary branches.
* **Raw View:** When viewing any file, click **Raw** to inspect unrendered content, including hidden comments.
* **Blame View:** Click **Blame** to see line-by-line commit authorship and timestamps.
* **Issues & Pull Requests:** Check both **Open** and **Closed** tabs to review past discussions, notes, and attachments.

---

### 2. GITHUB KEYBOARD SHORTCUTS

| Key | Action | Use Case |
| :--- | :--- | :--- |
| **`t`** | **File Finder** | Search and jump to any file in the repository instantly. |
| **`.` (Period)** | **Web Editor** | Opens the repository in browser-based VS Code for multi-file search (`Ctrl/Cmd + Shift + F`). |
| **`w`** | **Branch Switcher** | Opens the branch selection dropdown menu. |
| **`/`** or **`Cmd/Ctrl + K`** | **Search Bar** | Search code, commits, and discussions across the repository. |

---

### 3. ESSENTIAL TERMINAL COMMANDS

```bash
# View complete commit history across all branches
git log --oneline --graph --all

# Inspect exact changes (diffs) made in past commits
git log -p

# List all local and remote branches
git branch -a

# Switch to another branch
git checkout <branch-name>

# Search repository files for a specific keyword
git grep -i "<keyword>"

# Inspect details and diff of a specific commit
git show <commit-hash>
```
