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


Commit history before rebase:

<img width="791" height="208" alt="image" src="https://github.com/user-attachments/assets/4166903c-5bad-452f-867f-e52d6c31a6e3" />
![image_alt](https://github.com/ShoaibDevOps-star/ostadlab/blob/6fccc74dde6590032256c9451a3c063ba5a7d1d5/578117630-4166903c-5bad-452f-867f-e52d6c31a6e3.png)
Commit history after rebase:

<img width="811" height="213" alt="image" src="https://github.com/user-attachments/assets/7f117469-63ad-4f9b-b19f-33244b5f741f" />





