# Git Branching Strategy

## Introduction

Git branching allows developers to work on different features independently without affecting the stable version of the project.

## Branches Used in This Project

### 1. Main Branch
- Contains the stable version of the project.
- Used for production-ready code.

### 2. Dev Branch
- Used for development and integration.
- Receives completed feature branches through Pull Requests.

### 3. Feature Branch
- Created for developing individual features.
- Changes are reviewed before merging into the development branch.

## Workflow

1. Start from the dev branch.
2. Create a feature branch.
3. Implement the required changes.
4. Stage and commit changes.
5. Push the feature branch to GitHub.
6. Create a Pull Request targeting dev.
7. Review and merge the Pull Request.
8. Merge dev into main when the development work is ready.

## Git Commands

```bash
git switch dev
git pull origin dev
git switch -c feature/new-feature
git add .
git commit -m "Add new feature"
git push -u origin feature/new-feature
```

## Merge vs Rebase

### Merge
Combines changes from one branch into another and may create a merge commit.

### Rebase
Moves or replays commits onto a new base commit, creating a linear history.

## Conclusion

A proper branching strategy helps maintain organized development, improves collaboration, and protects the stable main branch.