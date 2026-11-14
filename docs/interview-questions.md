# Git Interview Questions

## 1. What is Git?

Git is a distributed version control system used to track changes in source code.
It helps developers collaborate, maintain project history, and manage different versions of files.

## 2. What is the difference between Git Merge and Git Rebase?

- Merge combines changes from different branches and creates a merge commit when necessary.
- Rebase moves commits onto a new base commit to create a linear history.

## 3. What is a Pull Request?

A Pull Request (PR) is a request to merge changes from one branch into another.
It allows team members to review code, discuss changes, and approve them before merging.

## 4. How do you resolve merge conflicts?

1. Run `git status` to identify conflicting files.
2. Open the conflicting files.
3. Find conflict markers such as `<<<<<<<`, `=======`, and `>>>>>>>`.
4. Edit the file to keep the correct content.
5. Run `git add <file>`.
6. Commit the resolved changes.

## 5. What are Git Tags?

Git tags are used to mark specific commits, usually for release versions.

Example:

`git tag -a v1.0.0 -m "First release"`

## 6. What is a Git Workflow?

A Git workflow is a structured process for managing development using branches, commits, pull requests, and merges.

Example:
- main: Stable code.
- dev: Development and integration.
- feature branches: Individual feature development.

## 7. What is Git Stash?

Git stash temporarily saves uncommitted changes so developers can switch branches without committing incomplete work.

Commands:

- `git stash` – Save changes.
- `git stash list` – View saved stashes.
- `git stash pop` – Restore the latest stash.

## 8. What is .gitignore?

`.gitignore` is a file that specifies files and directories Git should ignore.

Examples include:
- Environment files (`.env`)
- Dependencies (`node_modules/`)
- Python cache (`__pycache__/`)
- Temporary files (`*.log`)