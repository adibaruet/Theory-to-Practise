# Git Documentation

## Introduction
Git is a distributed version control system designed to handle everything from small to very large projects with speed and efficiency. It allows multiple developers to work on the same project without conflicts.

## Installation

### Windows
1. Download Git from [git-scm.com](https://git-scm.com/downloads).
2. Run the installer and follow the setup wizard.
3. Verify installation:
   ```sh
   git --version
   ```

### macOS
1. Install Git using Homebrew:
   ```sh
   brew install git
   ```
2. Verify installation:
   ```sh
   git --version
   ```

### Linux
1. Install Git using package manager:
   ```sh
   sudo apt install git   # Debian/Ubuntu
   sudo dnf install git   # Fedora
   sudo pacman -S git     # Arch
   ```
2. Verify installation:
   ```sh
   git --version
   ```

## Basic Git Commands

### Configuring Git
```sh
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Initializing a Repository
```sh
git init
```

### Cloning a Repository
```sh
git clone <repository-url>
```

### Checking Status
```sh
git status
```

### Adding Files to Staging Area
```sh
git add <file-name>  # Add a specific file
git add .            # Add all files
```

### Committing Changes
```sh
git commit -m "Commit message"
```

### Viewing Commit History
```sh
git log
```

### Pushing Changes to Remote Repository
```sh
git push origin main
```

### Pulling Changes from Remote Repository
```sh
git pull origin main
```

## Branching and Merging

### Creating a New Branch
```sh
git branch <branch-name>
```

### Switching to a Branch
```sh
git checkout <branch-name>
```

### Creating and Switching to a New Branch
```sh
git checkout -b <branch-name>
```

### Merging Branches
```sh
git checkout main
git merge <branch-name>
```

### Deleting a Branch
```sh
git branch -d <branch-name>
```

## Working with Remote Repositories

### Adding a Remote Repository
```sh
git remote add origin <repository-url>
```

### Viewing Remote Repositories
```sh
git remote -v
```

### Removing a Remote Repository
```sh
git remote remove origin
```

## Undoing Changes

### Undo Last Commit (Keep Changes in Staging)
```sh
git reset --soft HEAD~1
```

### Undo Last Commit (Discard Changes)
```sh
git reset --hard HEAD~1
```

### Remove a File from Staging
```sh
git reset HEAD <file-name>
```

### Revert a Commit
```sh
git revert <commit-hash>
```

## Git Ignore
Create a `.gitignore` file to exclude files from version control. Example:
```
node_modules/
*.log
.DS_Store
.env
```

## Git Tags

### Creating a Tag
```sh
git tag -a v1.0 -m "Version 1.0"
```

### Pushing Tags to Remote
```sh
git push origin v1.0
```

### Listing Tags
```sh
git tag
```

## Git Stash

### Save Uncommitted Changes
```sh
git stash
```

### Apply Stashed Changes
```sh
git stash apply
```

### Remove Stashed Changes
```sh
git stash drop
```

## Git Rebase

```sh
git checkout feature-branch
git rebase main
```

## Conclusion
Git is a powerful tool for version control. Mastering its commands and best practices will enhance collaboration and software development workflow.

For more information, visit [git-scm.com](https://git-scm.com/doc).
