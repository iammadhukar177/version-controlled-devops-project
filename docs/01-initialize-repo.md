# 🟢 Step 1: Initialize Git Repository

This guide explains how to initialize your Git project and push it to GitHub.

---

## 🔧 Steps to Initialize Git

```bash
# Create project folder
mkdir version-controlled-devops-project
cd version-controlled-devops-project

# Initialize Git
git init

# Add remote repository
git remote add origin https://github.com/<your-username>/<repo-name>.git

# Add files and make the first commit
echo "# DevOps Git Project" > README.md
touch .gitignore
git add .
git commit -m "Initial commit"

# Push to main branch
git branch -M main
git push -u origin main
