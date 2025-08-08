# 📁 Version-Controlled DevOps Project using Git

[![Git](https://img.shields.io/badge/Version%20Control-Git-blue?style=flat-square&logo=git)](https://git-scm.com/)  
[![GitHub](https://img.shields.io/badge/Hosted%20on-GitHub-black?style=flat-square&logo=github)](https://github.com/)  
[![DevOps](https://img.shields.io/badge/DevOps-Workflow-success?style=flat-square&logo=dev.to)](https://www.atlassian.com/devops)

---

## 🎯 Objective

This project demonstrates how to manage a DevOps project using **Git best practices**, including:

- Repository initialization
- Branching strategy
- Pull request workflows
- Semantic version tagging
- Markdown-based documentation

---

## 📌 Table of Contents

- [📁 Project Structure](#-project-structure)
- [🛠 Tools & Technologies](#-tools--technologies)
- [🔧 Step-by-Step Setup Guide](#-step-by-step-setup-guide)
  - [1. Initialize Git Repository](#1-initialize-git-repository)
  - [2. Implement Branching Strategy](#2-implement-branching-strategy)
  - [3. Create & Review Pull Requests](#3-create--review-pull-requests)
  - [4. Add Tags for Versioning](#4-add-tags-for-versioning)
  - [5. Document the Project](#5-document-the-project)
- [🐍 Sample App](#-sample-app)
- [✅ Git Best Practices Followed](#-git-best-practices-followed)
- [📄 Docs](#-docs)
- [📌 Future Enhancements](#-future-enhancements)

---

## 📁 Project Structure

```
version-controlled-devops-project/
├── .gitignore
├── README.md
├── docs/
│   ├── 01-initialize-repo.md
│   ├── 02-branching-strategy.md
│   ├── 03-pull-requests.md
│   ├── 04-tags.md
│   └── 05-git-best-practices.md
└── sample-app/
    └── app.py
```

---

## 🛠 Tools & Technologies

| Tool         | Description                     |
|--------------|----------------------------------|
| **Git**      | Version control system           |
| **GitHub**   | Remote code hosting              |
| **Markdown** | Documentation format             |
| **Python**   | For sample app demonstration     |

---

## 🔧 Step-by-Step Setup Guide

### ✅ 1. Initialize Git Repository

```bash
mkdir version-controlled-devops-project && cd version-controlled-devops-project
git init
echo "# Version-Controlled DevOps Project" > README.md
echo "__pycache__/
.env
*.log
*.pyc" > .gitignore
git remote add origin https://github.com/<your-username>/<repo-name>.git
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
```

---

### ✅ 2. Implement Branching Strategy

```bash
# Create and push dev branch
git checkout -b dev
git push -u origin dev

# Create a feature branch
git checkout -b feature/sample-app dev
```

📌 **Branching Model**:
- `main`: production/stable
- `dev`: integration branch
- `feature/*`: for new features

---

### ✅ 3. Create & Review Pull Requests

1. Push your feature branch:
   ```bash
   git push origin feature/sample-app
   ```
2. Open a PR on GitHub:
   - From `feature/sample-app` ➝ `dev`
   - After review, merge `dev` ➝ `main`

💡 Use **Squash & Merge** or **Rebase** for clean history.

---

### ✅ 4. Add Tags for Versioning

```bash
# Create annotated tag
git checkout main
git tag -a v1.0 -m "First stable release"
git push origin v1.0
```

🏷️ Use **semantic versioning**: `v1.0.0`, `v1.1.0`, `v2.0.0`, etc.

---

### ✅ 5. Document the Project

All workflows and strategies are documented in the `docs/` folder using markdown.

| Doc File                     | Description                    |
|-----------------------------|--------------------------------|
| `01-initialize-repo.md`     | Git setup instructions         |
| `02-branching-strategy.md`  | Git flow and branching rules   |
| `03-pull-requests.md`       | PR creation and review guide   |
| `04-tags.md`                | Version tagging instructions   |
| `05-git-best-practices.md`  | Professional Git usage tips    |

---

## 🐍 Sample App

```python
# sample-app/app.py

def hello():
    return "Hello from DevOps Git project!"

if __name__ == "__main__":
    print(hello())
```

Used as a dummy application to demonstrate version control over a project file.

---

## ✅ Git Best Practices Followed

- Meaningful, atomic commits
- Branching model: `main` / `dev` / `feature/*`
- Code collaboration via pull requests
- Semantic tagging for releases
- Markdown documentation
- Sensitive files excluded via `.gitignore`

---

## 📄 Docs

Inside `docs/`, you'll find step-by-step guides for each phase of this project:

- ✔️ Git init & remote setup
- ✔️ Branching strategy
- ✔️ Creating & merging PRs
- ✔️ Semantic tagging
- ✔️ Git best practices checklist

---

## 📌 Future Enhancements

- [ ] Add GitHub Actions for CI
- [ ] Use Docker to containerize the sample app
- [ ] Add issue templates and PR templates
- [ ] Implement Git hooks for linting

---

## 🧠 Author & Credits

Created by **Madhukar Sammeta** — DevOps Engineer & Full Stack Developer  
🌐 Portfolio: [coming soon]  
📧 Contact: madhukar.sammeta@example.com

---

> “Version control isn't just about saving code — it's about working better, together.”  
> — *DevOps Philosophy*
