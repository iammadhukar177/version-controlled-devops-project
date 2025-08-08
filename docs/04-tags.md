# 🏷️ Step 4: Tags for Versioning

Tags help mark specific points in Git history like releases or milestones.

---

## 🛠 How to Tag a Release

```bash
# Move to the main branch
git checkout main

# Add a tag with a message
git tag -a v1.0 -m "Initial stable release"

# Push the tag to remote
git push origin v1.0
