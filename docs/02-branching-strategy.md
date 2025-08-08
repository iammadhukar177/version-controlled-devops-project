
---

### ✅ `docs/02-branching-strategy.md`

```markdown
# 🌿 Step 2: Branching Strategy

In DevOps, following a good branching strategy ensures smooth collaboration and code quality.

---

## 🔄 Branch Types

- `main`: Stable, production-ready code
- `dev`: Ongoing development and integration
- `feature/<feature-name>`: Used for new features

---

## 🔧 Commands to Create Branches

```bash
# Create and push dev branch
git checkout -b dev
git push -u origin dev

# Create a new feature branch from dev
git checkout -b feature/sample-app dev
