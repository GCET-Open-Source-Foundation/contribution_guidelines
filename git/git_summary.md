# Git: Your Friendly Time Machine for Code

---

## Before You Delve In

This doc gives you a short summary of Git, why it matters, and the core commands you will use every day.
A small tutorial at the end shows you how to try them yourself.

---

## What is Git?

Git is a distributed version control system (DVCS).
In plain English: it is a tool that lets you track changes in your code, experiment safely, and collaborate with others without losing your work.

Think of it as a time machine: every time you save with `git commit -s -m "message"`, you take a snapshot of your project that you can always come back to.

---

## Official Definition

From the [Git project site](https://git-scm.com):

> "Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency."

---

## Why Use Git?

* History you can trust: roll back to any version of your project, any time
* Freedom to experiment: create branches (alternate timelines) to test new ideas without breaking the main project
* Collaboration made simple: multiple developers can work on the same codebase, merge changes, and resolve conflicts in an organized way
* Offline-first: you do not need internet to use Git, everything is saved locally, you sync later
* Industry standard: if you are coding with others, Git (and GitHub) is the language everyone speaks

---

## Core Commands

```bash
git init                 # start a new repo
git clone URL            # copy an existing repo
git status               # check what has changed
git add file             # stage a file
git commit -s -m "msg"   # save a signed snapshot
git push                 # send changes to remote (e.g. GitHub)
git pull                 # fetch and merge changes from remote
git checkout -b branch   # make a new branch
git merge branch         # merge a branch back
```

---

## Quick Tutorial

Try this to see Git in action:

```bash
# 1. Create a new folder and move into it
mkdir git-demo && cd git-demo

# 2. Initialize Git
git init

# 3. Create a file
echo "Hello Git" > hello.txt

# 4. Check status
git status

# 5. Stage the file
git add hello.txt

# 6. Commit with sign-off
git commit -s -m "Add hello.txt"

# 7. Create a new branch
git checkout -b experiment

# 8. Edit the file
echo "Another line" >> hello.txt

# 9. Commit again
git add hello.txt
git commit -s -m "Update hello.txt with another line"

# 10. Switch back and merge
git checkout main
git merge experiment
```

With that, you have:

* created a repo
* made commits with sign-off
* experimented in a branch
* merged changes back

---

## Wrap Up

Git is your project’s time machine. It protects your work, lets you experiment without fear, and makes collaboration easier.
Once you are comfortable with these basics, you can move on to branching strategies, rebasing, and more advanced workflows.

