# Git & GitHub Essentials

[![Download](https://img.shields.io/badge/Download-GIT-blue?style=for-the-badge&logo=github)](https://git-scm.com/downloads)

A clean, practical Git + GitHub guide for daily use.

---

## 📑 Table of Contents

- [🔧 Git Daily Commands](#-git-daily-commands)
  - [🔁 Basic Workflow](#basic-workflow)
  - [🌿 Branching](#branching)
  - [🧹 Reset & Clean](#reset--clean)
  - [📜 Logs & History](#logs--history)
  - [🔍 Search & Inspect](#search--inspect)
  - [🌐 Remote Management](#remote-management)
- [✅ Best Practices](#best-practices)
- [📁 .gitignore Example](#gitignore-example)
- [⚡ Git Aliases](#git-aliases)
- [🔗 Useful Links](#useful-links)

---

## 🔧 Git Daily Commands

<details id="basic-workflow">
<summary>🔁 <strong>Basic Workflow</strong></summary>

*initialize a new repository*
```bash
git init
````

*clone a remote repository*

```bash
git clone <repo_url>
```

*check the status of changes*

```bash
git status
```

*stage a specific file or directory*

```bash
git add <file_or_folder>
```

*stage all changes*

```bash
git add .
```

*commit staged changes with a message*

```bash
git commit -m "your message"
```

*push commits to remote*

```bash
git push
```

*pull latest changes and merge*

```bash
git pull
```

</details>

---

<details id="branching">
<summary>🌿 <strong>Branching</strong></summary>

*list all local branches*

```bash
git branch
```

*create a new branch*

```bash
git branch <branch_name>
```

*switch to a branch*

```bash
git checkout <branch_name>
```

*create and switch to a new branch*

```bash
git checkout -b <branch_name>
```

*merge another branch into the current branch*

```bash
git merge <branch_name>
```

</details>

---

<details id="reset--clean">
<summary>🧹 <strong>Reset & Clean</strong></summary>

*discard local changes in a file*

```bash
git restore <file>
```

*unstage a file without discarding changes*

```bash
git reset HEAD <file>
```

*reset all changes (dangerous)*

```bash
git reset --hard
```

*remove all untracked files and folders*

```bash
git clean -fd
```

</details>

---

<details id="logs--history">
<summary>📜 <strong>Logs & History</strong></summary>

*view full commit history*

```bash
git log
```

*compact commit history with graph*

```bash
git log --oneline --graph
```

*show changes not staged for commit*

```bash
git diff
```

*show staged changes*

```bash
git diff --staged
```

</details>

---

<details id="search--inspect">
<summary>🔍 <strong>Search & Inspect</strong></summary>

*show full details of a commit*

```bash
git show <commit_hash>
```

*see who last modified each line of a file*

```bash
git blame <file>
```

</details>

---

<details id="remote-management">
<summary>🌐 <strong>Remote Management</strong></summary>

*list all remotes*

```bash
git remote -v
```

*add a remote repository*

```bash
git remote add origin <repo_url>
```

*push and set upstream tracking*

```bash
git push -u origin <branch_name>
```

</details>

---

## ✅ Best Practices

<details id="best-practices">
<summary><strong>Best Practices</strong></summary>

### 🧼 Commits

* use small, focused commits
* write clear messages in imperative form: `add login page`, `fix header`
* avoid committing unnecessary or temporary files

### 🌿 Branches

* use descriptive names like `feature/navbar`, `fix/modal`
* avoid direct commits to `main` or `master`
* delete merged branches regularly

### 🧪 Before Pushing

* `git pull --rebase` to sync before pushing
* test your code and check `git diff --staged`
* keep your commit history clean and readable

### 🤝 Collaboration

* use pull requests for every merge
* write clear PR titles/descriptions
* request and provide reviews

### 🚨 Safety

* never commit secrets or config files
* use `.gitignore` effectively
* avoid `--force` unless absolutely necessary

</details>

---

## 📁 .gitignore Example

<details id="gitignore-example">
<summary><strong>.gitignore Example</strong></summary>

```gitignore
# node / js
node_modules/
dist/
*.log

# system files
.DS_Store
*.swp

# environment / secrets
.env
.env.*
```

</details>

---

## ⚡ Git Aliases

<details id="git-aliases">
<summary><strong>Git Aliases</strong></summary>

```bash
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.cm "commit -m"
git config --global alias.lg "log --oneline --graph --all"
```

</details>

---

## 🔗 Useful Links

<details id="useful-links">
<summary><strong>Useful Links</strong></summary>

* [Git Docs](https://git-scm.com/doc)
* [GitHub Docs](https://docs.github.com/)
* [Git Cheat Sheet PDF](https://education.github.com/git-cheat-sheet-education.pdf)
* [Pro Git Book (Free)](https://git-scm.com/book/en/v2)
* [Learn Git Branching (Interactive)](https://learngitbranching.js.org/)
* [Oh My Git! (Game)](https://ohmygit.org/)

</details>

---

> 📘 Bookmark or clone this repo and use it as your go-to Git reference.
