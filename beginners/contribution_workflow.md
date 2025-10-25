# Contribution Flow

Before you delve this document explains the exact steps
to contribute to GCET-OSS projects. Follow these steps
carefully so your contribution can be reviewed and merged
smoothly.

Starting out here are some steps:

---

## 1. Fork the Repository

Go to the GitHub repository you want to contribute to and
click **Fork**.
This creates a copy of the repository under your account.

---

## 2. Clone the Repository

Clone your fork to your local machine.

```
git clone https://github.com/your-username/repository-name.git
cd repository-name
```

---

## 3. Add the Upstream Remote

Point your local copy to the original GCET-OSS repository
so you can sync changes later.

```
git remote add upstream https://github.com/GCET-OSS/repository-name.git
```

---

## 4. Create a New Branch

Always create a new branch for your work. Do not work directly
on the `main` branch.

```
git checkout -b feature-branch-name
```

Branch names should be short and descriptive, for example:

```
fix-typo-readme
add-login-component
update-go-function
```

---

## 5. Make Your Changes

Edit the code, documentation, or configuration as required.
Keep your changes focused. One pull request should solve one
issue or add one feature.

---

## 6. Stage and Commit

Add the files you changed and commit with a clear message.

```
git add .
git commit -s
It opens an editor, type your commit message in the following format:
Begin with an imperative or commanding statement — use words like Add, Fix, Change, etc.

Then, describe the current behavior of the system and clearly highlight the issue within it.

Next, propose a solution that addresses the described issue.

Finally, demonstrate how your changes or code snippets have affected the results of the codebase.

Note: Do not describe what you’ve done; instead, describe why you’ve done it.
```

A good commit message describes **why** you changed, not just
“fixed” or **what**.

---

## 7. Push to Your Fork

Push your branch to your GitHub fork.

```
git push origin feature-branch-name
```

---

## 8. Open a Pull Request

Go to your fork on GitHub.
Click **Compare & Pull Request**.
Write a clear title and description for your pull request,
linking it to the related issue if one exists.

Example:

```
- Give an observation on how the current system works in the
   present tense (so no need to say "Currently X is Y", or
   "Previously X was Y" to describe the state before your change;
   just "X is Y" is enough), and discuss what you perceive as a
   problem in it.

- Propose a solution (optional---often, problem description
   trivially leads to an obvious solution in reader's minds).

- Give commands to the codebase to "become like so".
```

---

## 9. Review and Feedback

Maintainers will review your pull request. They may request
changes.
Update your branch as needed, then push again. The pull request
will update automatically.

---

## 10. Merge

Once approved, a maintainer will merge your changes into the
repository.
Congratulations, you are now a contributor to GCET-OSS.

---

## 11. Keep Your Fork Updated

Regularly sync your fork to stay up to date.

```
git checkout main
git pull upstream main
git push origin main
```

---

This is the standard contribution flow for GCET-OSS projects.
Following these steps ensures that contributions are clean,
consistent, and easy to review.
