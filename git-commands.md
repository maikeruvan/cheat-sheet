
## 🌟 Starting Fresh

* `git init`
  * Turns your current local folder into a brand new, empty Git repository.
* `git clone <url>`
  * Downloads an existing project from GitHub onto your computer.
* `git clone <url> .`
  * Downloads a project directly into your current active terminal folder without creating a new subfolder.

---

## 📝 Making Changes (The Daily Cycle)

* `git status`
  * **Your best friend.** Shows which files you edited, deleted, or haven't tracked yet.
* `git add <filename>`
  * Prepares a specific file to be saved (stages it).
* `git add .`
  * Prepares **all** modified and new files to be saved at once.
* `git commit -m "your message"`
  * Permanently saves your staged changes into Git history with a descriptive note.

---

## 🌿 Working with Branches

* `git branch`
  * Lists all local branches on your computer. (The one with the `*` is where you are currently standing).
* `git checkout -b <branch-name>`
  * Creates a brand new branch and switches you into it immediately.
* `git checkout <branch-name>`
  * Switches you back to an existing branch (e.g., `git checkout main`).

---

## 🤝 Merging & Cleaning Up (Locally)

* `git merge <branch-name>`
  * Combines another branch's changes into your *current* active branch.
* `git merge --no-ff <branch-name>`
  * **Forces a explicit merge commit.** Prevents Git from fast-forwarding, leaving a visual trail proving the work came from a separate branch.
* `git branch -d <branch-name>`
  * Deletes a local branch (safely checks if it was merged first).
* `git branch -D <branch-name>`
  * **Force-deletes** a local branch, discarding any unmerged work.

---

## ☁️ Talking to GitHub (The Cloud)

* `git push origin <branch-name>`
  * Uploads your local commits up to your repository on GitHub.
* `git pull origin <branch-name>`
  * Downloads and merges the latest changes from GitHub straight into your current local branch.
* `git config --global pull.rebase false`
  * **The non-rebase fix.** Configures Git to always use standard merging when pulling down code, silencing the annoying warning Git shows when you pull.
* `git pull origin main --no-rebase`
  * **The Conflict Pull.** Forces Git to execute a traditional merge when downloading changes from GitHub, letting you see and resolve conflicts directly inside VS Code if the cloud and local files don't match.

---

## 🚨 Oops, I Made a Mistake! (The Safety Nets)

* `git log --oneline`
  * Shows a neat, simplified history list of your recent commits.
* `git reflog`
  * The hidden diary that shows a list of every single action you took (good for 30–90 days).
* `git checkout -- <filename>`
  * Discards unsaved changes in a file and reverts it back to how it looked at your last commit.
