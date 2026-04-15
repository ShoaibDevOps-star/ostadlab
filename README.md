# Git Branching & Commit Management Project

## 📋 Project Overview
This project demonstrates advanced Git workflows including:
- Multi-branch management
- Merge vs Rebase strategies
- Interactive rebase with squash and reword operations
- GitHub Pull Request workflow

## 🔗 Repository Link
**GitHub Repository:** `https://github.com/ShoaibDevOps-star/ostadlab.git`

---

## 📝 All Commands Used

### 1. Repository Initialization & Branch Creation

```bash
# Create and initialize repository
mkdir ostadlab
cd ostadlab
git init

# Create branches
git checkout -b main
git branch develop
git branch feature/login
git branch feature/payment
git branch feature/profile
git branch bugfix/login-error

# Verify branches
git branch
# Output:
#   bugfix/login-error
#   develop
#   feature/login
#   feature/payment
#   feature/profile
# * main
```
<img width="836" height="168" alt="image" src="https://github.com/user-attachments/assets/93cd368f-b862-4a2e-952d-5201e700a55b" />

Commit history before rebase:

pick 8bff2ec Add First login HTML file
pick 409ba0f Add Second login HTML file
pick 0647b73 Add Third login HTML file
pick 52fc3ae Add Six login HTML file
pick 8fed436 Add Second login HTML file
pick 5000f5a Add Third login HTML file
pick 1232a80 Add Fourth login HTML file
pick 2cd5233 Add Fifth login HTML file
pick 4faade3 Add Six login HTML file

<img width="791" height="208" alt="image" src="https://github.com/user-attachments/assets/4166903c-5bad-452f-867f-e52d6c31a6e3" />

Commit history after rebase:

pick 8bff2ec Add First login HTML file
pick 409ba0f Add Second login HTML file
pick 0647b73 Add Third login HTML file
pick 52fc3ae Add Six login HTML file
squash 8fed436 Add Second login HTML file
squash 5000f5a Add Third login HTML file
reword 1232a80 Add Fourth login HTML file and rewrite messages
pick 2cd5233 Add Fifth login HTML file
squash 4faade3 Add Six login HTML file

<img width="811" height="213" alt="image" src="https://github.com/user-attachments/assets/7f117469-63ad-4f9b-b19f-33244b5f741f" />


Git Merge 🤝

What it does:
Merge creates a new "merge commit" that joins two branches together, preserving the complete history of both branches.

Git Rebase 🔄

What it does:
Rebase moves the entire feature branch to begin at the tip of the target branch, creating a linear history.

<img width="836" height="291" alt="image" src="https://github.com/user-attachments/assets/bf5c1afe-6c13-425f-9e24-6993e59c8217" />


Squash 📦

What it does:
Squash combines multiple commits into a single commit, allowing you to create a cleaner, more meaningful commit history.

Reword ✏️

What it does:
Reword allows you to change the message of an existing commit without changing its content.

When to use Squash:

    ✅ Cleaning up "WIP" (Work In Progress) commits

    ✅ Combining related fixes and adjustments

    ✅ Before creating pull requests

    ✅ When commits break down into logical units
    
When to use Reword:

    ✅ Fixing typos in commit messages

    ✅ Making commit messages more descriptive

    ✅ Adding missing context or ticket numbers

    ✅ Standardizing message format

    ✅ Clarifying what changed and why


