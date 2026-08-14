---
title: "Untitled note"
tags: []
date: 2026-08-14
folder: work/test-notes-01
---

# 1. Learn the Basics

# Module 1: Learn the Basics

Welcome! This is the foundation. Everything else builds on these simple ideas.

---
"""python
## 1.1 What is Version Control?

**Simple explanation**  

Version Control is like a **time machine + backup system** for your code (or any files).
"""
It remembers every change you make, who made it, and when. You can go back to any previous version if something breaks.

**Real-life analogy**  

Think of Google Docs version history — but for your entire project, and it works offline + with teams.

### Examples

**Example 1 – Solo developer**  

You are writing a website. Yesterday the homepage looked perfect. Today you accidentally deleted the navigation bar. With version control you type one command and the perfect version comes back.

**Example 2 – Team of 3**  

Alice adds a login page, Bob adds a shopping cart, Charlie fixes a bug — all at the same time. Version control merges their work without overwriting each other.

**Example 3 – Open source**  

Thousands of people contribute to React or VS Code. Version control (Git) is the only reason this is possible without total chaos.

---

## 1.2 Why use Version Control?

### Top reasons (beginner friendly)

1. **Never lose work** – Every save is permanent history
2. **Experiment safely** – Create a "branch" (copy) and try crazy ideas. If it fails → delete the branch
3. **Collaborate without fear** – Multiple people edit the same project
4. **See who changed what** – Great for debugging and learning
5. **Release versions** – Tag v1.0, v1.1, etc. easily

### Real-time examples

**Example 1 – Broken CSS**  

You change colors and the site looks ugly. Instead of undoing 20 lines manually:

```bash
git checkout -- style.css
```

Instant restore.

**Example 2 – Feature experiment**  

You want to try a dark mode. Create a branch `dark-mode`, experiment freely. Client hates it → delete branch. Main site is untouched.

**Example 3 – Client change request**  

Client says "go back to the version from last Friday". With Git you can show them exactly that version in seconds.

---

## 1.3 Git vs Other VCS

| Feature | Git (Distributed) | SVN / Centralized | Why Git wins for most people |
| --- | --- | --- | --- |
| Offline work | Full history offline | Needs server | You can commit on a plane |
| Speed | Extremely fast | Slower | Local operations |
| Branching | Super cheap & easy | Expensive | Branch for every feature |
| Popularity | Industry standard | Declining | Almost every company uses it |
| Learning curve | Medium | Easier at first | Worth it long-term |

**Git** is a **Distributed Version Control System (DVCS)**.  

Every developer has the complete history on their computer.

**Other systems** (like Subversion) are centralized — the server holds the "truth".

### Examples

**Example 1**  

You are on a train with no internet. With Git you can still commit, create branches, look at history. With SVN you are stuck.

**Example 2**  

GitHub, GitLab, Bitbucket all use Git under the hood. Learning Git = learning the tool behind 95% of modern software.

**Example 3**  

Even huge companies (Google, Microsoft, Facebook) use Git (or Git-based systems).

---

## 1.4 Installing Git Locally

### Windows

1. Go to [https://git-scm.com/download/win](https://git-scm.com/download/win)
2. Download the installer
3. Keep all default options (especially "Git from the command line")
4. Finish → Open **Git Bash** or PowerShell and type:

```bash
git --version
```

You should see something like `git version 2.45.0`

### macOS

```bash
# Option A – Official installer
# Download from https://git-scm.com/download/mac

# Option B – Homebrew (recommended)
brew install git

git --version
```

### Linux (Ubuntu/Debian)

```bash
sudo apt update
sudo apt install git
git --version
```

### First-time configuration (do this once)

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Optional but recommended
git config --global init.defaultBranch main
git config --global core.editor "code --wait"   # if you use VS Code
```

**Verify**

```bash
git config --list --show-origin
```

### Practice Exercise

1. Install Git
2. Set your name and email
3. Create a folder `~/git-practice`
4. Inside it run `git --version` and screenshot / note the output

---

**Next Module → Repositories & Core Commands**

You now understand *why* we use Git. Time to actually use it!

