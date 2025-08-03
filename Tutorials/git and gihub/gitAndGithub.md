# 🚀 Git and GitHub Complete Guide

Git is a distributed version control system that helps developers track changes in their code, collaborate with others, and maintain a complete history of their project. GitHub is a web-based platform that hosts Git repositories and provides additional collaboration features.

---

## ❓ Question 1: What is Git and Why Do We Need It?

### 🎯 What is Git?

Git is a **distributed version control system** created by Linus Torvalds in 2005. It allows developers to track changes in their code, collaborate with others, and maintain a complete history of their project.

### 🔍 Why Do We Need Version Control?

#### **Without Version Control:**
```
project_v1.txt
project_v2.txt
project_v2_final.txt
project_v2_final_really.txt
project_v2_final_really_this_time.txt
```

#### **With Git:**
```bash
# Clean, organized history
git log --oneline
# a1b2c3d Latest feature
# e4f5g6h Bug fix
# h7i8j9k Initial commit
```

### 🎯 Key Benefits of Git

#### **1. Version History**
- **Track every change** made to your code
- **Revert to any previous version** if something breaks
- **See who made what changes** and when

#### **2. Collaboration**
- **Multiple people** can work on the same project
- **Merge changes** from different developers
- **Resolve conflicts** when changes overlap

#### **3. Backup and Safety**
- **Complete backup** of your project
- **Work offline** and sync later
- **Never lose your work** again

#### **4. Branching and Experimentation**
- **Try new features** without breaking existing code
- **Work on different features** simultaneously
- **Safe experimentation** with new ideas

### 🏗️ How Git Works

#### **Three Main Areas:**
```bash
Working Directory  →  Staging Area  →  Repository
     (Files)           (Index)         (History)
```

#### **Git Workflow:**
1. **Working Directory:** Where you edit files
2. **Staging Area:** Where you prepare changes for commit
3. **Repository:** Where Git stores the complete history

---

## ❓ Question 2: What is GitHub and How Does it Relate to Git?

### 🌐 What is GitHub?

GitHub is a **web-based platform** that hosts Git repositories and provides additional collaboration features. It's like "social media for code" where developers can share, collaborate, and contribute to projects.

### 🔗 Git vs GitHub

| Feature | Git | GitHub |
|---------|-----|--------|
| **Type** | Version control system | Web platform |
| **Location** | Local on your computer | Remote on the internet |
| **Purpose** | Track changes locally | Host and share repositories |
| **Features** | Basic version control | Collaboration, issues, pull requests |

### 🚀 GitHub Features

#### **1. Repository Hosting**
- **Store your Git repositories** online
- **Access from anywhere** with internet
- **Backup your code** in the cloud

#### **2. Collaboration Tools**
- **Pull Requests** - Review and merge code changes
- **Issues** - Track bugs and feature requests
- **Discussions** - Communicate with team members
- **Projects** - Organize and track work

#### **3. Social Features**
- **Follow other developers** and projects
- **Star repositories** you like
- **Fork projects** to contribute
- **Discover new projects** and libraries

#### **4. Integration**
- **CI/CD pipelines** (GitHub Actions)
- **Code review** tools
- **Documentation** hosting
- **Package publishing**

---

## ❓ Question 3: How to Install and Configure Git?

### 🛠️ Installing Git

#### **Windows:**
```bash
# Download from git-scm.com
# Or use Chocolatey
choco install git

# Or use winget
winget install Git.Git
```

#### **macOS:**
```bash
# Using Homebrew
brew install git

# Or download from git-scm.com
```

#### **Linux (Ubuntu/Debian):**
```bash
sudo apt update
sudo apt install git
```

#### **Linux (CentOS/RHEL):**
```bash
sudo yum install git
# or
sudo dnf install git
```

### ⚙️ Configuring Git

#### **Set Your Identity:**
```bash
# Set your name
git config --global user.name "Your Name"

# Set your email
git config --global user.email "your.email@example.com"

# Verify your settings
git config --list
```

#### **Configure Default Editor:**
```bash
# Set VS Code as default editor
git config --global core.editor "code --wait"

# Set Vim as default editor
git config --global core.editor "vim"

# Set Nano as default editor
git config --global core.editor "nano"
```

#### **Configure Default Branch:**
```bash
# Set main as default branch
git config --global init.defaultBranch main
```

#### **Configure Line Endings:**
```bash
# Windows
git config --global core.autocrlf true

# macOS/Linux
git config --global core.autocrlf input
```

### 🔑 Setting Up SSH Keys (Optional but Recommended)

#### **Generate SSH Key:**
```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "your.email@example.com"

# Start SSH agent
eval "$(ssh-agent -s)"

# Add SSH key to agent
ssh-add ~/.ssh/id_ed25519
```

#### **Add SSH Key to GitHub:**
```bash
# Copy public key
cat ~/.ssh/id_ed25519.pub

# Add to GitHub: Settings → SSH and GPG keys → New SSH key
```

#### **Test SSH Connection:**
```bash
ssh -T git@github.com
```

---

## ❓ Question 4: How to Create Your First Git Repository?

### 🏗️ Creating a New Repository

#### **Method 1: Initialize Local Repository**
```bash
# Create a new directory
mkdir my-project
cd my-project

# Initialize Git repository
git init

# Check repository status
git status
```

#### **Method 2: Clone Existing Repository**
```bash
# Clone from GitHub
git clone https://github.com/username/repository.git

# Clone with SSH
git clone git@github.com:username/repository.git

# Clone specific branch
git clone -b branch-name https://github.com/username/repository.git
```

### 📁 Understanding Repository Structure

#### **After git init:**
```
my-project/
├── .git/          # Git repository data (hidden)
└── (your files)
```

#### **After adding files:**
```
my-project/
├── .git/          # Git repository data
├── README.md      # Project documentation
├── index.html     # Your project files
├── style.css
└── script.js
```

### 🎯 Your First Commit

#### **Step 1: Create Files**
```bash
# Create a README file
echo "# My First Git Project" > README.md

# Create some project files
touch index.html style.css script.js
```

#### **Step 2: Check Status**
```bash
git status
# Output:
# Untracked files:
#   README.md
#   index.html
#   style.css
#   script.js
```

#### **Step 3: Add Files to Staging**
```bash
# Add specific file
git add README.md

# Add multiple files
git add index.html style.css

# Add all files
git add .

# Check staged files
git status
```

#### **Step 4: Commit Changes**
```bash
# Commit with message
git commit -m "Initial commit: Add project files"

# Check commit history
git log --oneline
```

---

## ❓ Question 5: What are the Basic Git Commands and How to Use Them?

### 📋 Essential Git Commands

#### **1. git status**
```bash
# Check repository status
git status

# Short status
git status -s
# Output: M  modified_file.txt
#         A  new_file.txt
#         D  deleted_file.txt
```

#### **2. git add**
```bash
# Add specific file
git add filename.txt

# Add multiple files
git add file1.txt file2.txt

# Add all files
git add .

# Add all tracked files (modified files)
git add -u

# Interactive add
git add -i
```

#### **3. git commit**
```bash
# Commit with message
git commit -m "Add new feature"

# Commit all tracked files (skip staging)
git commit -am "Update existing files"

# Amend last commit
git commit --amend -m "Updated commit message"

# Commit with detailed message
git commit
# Opens editor for longer message
```

#### **4. git log**
```bash
# Show commit history
git log

# One line per commit
git log --oneline

# Show last 5 commits
git log -5

# Show commits with files changed
git log --stat

# Show commits with patches
git log -p

# Show commits by author
git log --author="John Doe"

# Show commits since date
git log --since="2023-01-01"
```

#### **5. git diff**
```bash
# Show unstaged changes
git diff

# Show staged changes
git diff --staged

# Show changes in specific file
git diff filename.txt

# Show changes between commits
git diff commit1 commit2

# Show changes in last commit
git diff HEAD~1
```

### 🔄 Working with Files

#### **6. git rm**
```bash
# Remove file from Git and filesystem
git rm filename.txt

# Remove file from Git only (keep in filesystem)
git rm --cached filename.txt

# Remove directory
git rm -r directory/
```

#### **7. git mv**
```bash
# Rename file
git mv oldname.txt newname.txt

# Move file to different directory
git mv file.txt directory/file.txt
```

#### **8. git checkout**
```bash
# Discard changes in working directory
git checkout -- filename.txt

# Switch to specific commit
git checkout commit_hash

# Switch to specific branch
git checkout branch_name

# Create and switch to new branch
git checkout -b new_branch_name
```

#### **9. git reset**
```bash
# Unstage files (keep changes)
git reset HEAD filename.txt

# Reset to specific commit (keep changes)
git reset --soft commit_hash

# Reset to specific commit (discard changes)
git reset --hard commit_hash

# Reset last commit (keep changes)
git reset --soft HEAD~1
```

---

## ❓ Question 6: How to Work with Branches in Git?

### 🌿 What are Branches?

Branches are **parallel versions** of your code that allow you to work on features without affecting the main codebase. Think of them as separate timelines for your project.

### 🎯 Branch Concepts

#### **Main Branch (Default)**
```bash
# Usually called 'main' or 'master'
# Contains stable, production-ready code
# Should always be working
```

#### **Feature Branches**
```bash
# Temporary branches for new features
# Created from main branch
# Merged back when feature is complete
```

### 🌿 Branch Commands

#### **1. git branch**
```bash
# List all branches
git branch

# List all branches (local and remote)
git branch -a

# Create new branch
git branch feature-name

# Delete branch
git branch -d branch-name

# Force delete branch
git branch -D branch-name

# Rename current branch
git branch -m new-name
```

#### **2. git checkout**
```bash
# Switch to existing branch
git checkout branch-name

# Create and switch to new branch
git checkout -b new-branch-name

# Switch to previous branch
git checkout -
```

#### **3. git switch (Newer Git versions)**
```bash
# Switch to existing branch
git switch branch-name

# Create and switch to new branch
git switch -c new-branch-name

# Switch to previous branch
git switch -
```

### 🔄 Branch Workflow Example

#### **Step 1: Create Feature Branch**
```bash
# Ensure you're on main branch
git checkout main

# Create and switch to feature branch
git checkout -b add-login-feature
```

#### **Step 2: Work on Feature**
```bash
# Make changes to files
echo "// Login functionality" >> login.js

# Add and commit changes
git add login.js
git commit -m "Add login functionality"
```

#### **Step 3: Switch Between Branches**
```bash
# Switch back to main for urgent fix
git checkout main

# Make urgent fix
echo "// Bug fix" >> bugfix.js
git add bugfix.js
git commit -m "Fix urgent bug"

# Switch back to feature branch
git checkout add-login-feature
```

#### **Step 4: Merge Feature**
```bash
# Switch to main branch
git checkout main

# Merge feature branch
git merge add-login-feature

# Delete feature branch
git branch -d add-login-feature
```

### 🔀 Advanced Branch Operations

#### **git merge**
```bash
# Merge branch into current branch
git merge branch-name

# Merge with no fast-forward
git merge --no-ff branch-name

# Abort merge if conflicts
git merge --abort
```

#### **git rebase**
```bash
# Rebase current branch onto main
git rebase main

# Interactive rebase
git rebase -i HEAD~3

# Abort rebase
git rebase --abort
```

#### **Resolving Merge Conflicts**
```bash
# When merge conflict occurs
<<<<<<< HEAD
// Your changes
=======
// Their changes
>>>>>>> branch-name

# Edit file to resolve conflict
# Remove conflict markers
# Add resolved file
git add filename.txt
git commit -m "Resolve merge conflict"
```

---

## ❓ Question 7: How to Work with Remote Repositories (GitHub)?

### 🌐 Understanding Remote Repositories

Remote repositories are **Git repositories hosted on servers** (like GitHub, GitLab, Bitbucket) that allow collaboration and backup of your code.

### 🔗 Remote Repository Commands

#### **1. git remote**
```bash
# List remote repositories
git remote

# List remote repositories with URLs
git remote -v

# Add remote repository
git remote add origin https://github.com/username/repository.git

# Remove remote repository
git remote remove origin

# Rename remote repository
git remote rename origin upstream
```

#### **2. git clone**
```bash
# Clone repository
git clone https://github.com/username/repository.git

# Clone to specific directory
git clone https://github.com/username/repository.git my-directory

# Clone specific branch
git clone -b branch-name https://github.com/username/repository.git

# Clone with SSH
git clone git@github.com:username/repository.git
```

#### **3. git fetch**
```bash
# Fetch updates from remote
git fetch origin

# Fetch specific branch
git fetch origin branch-name

# Fetch all remotes
git fetch --all
```

#### **4. git pull**
```bash
# Pull changes from remote
git pull origin main

# Pull and rebase
git pull --rebase origin main

# Pull specific branch
git pull origin feature-branch
```

#### **5. git push**
```bash
# Push to remote
git push origin main

# Push new branch
git push origin new-branch

# Push and set upstream
git push -u origin branch-name

# Force push (use with caution)
git push --force origin branch-name
```

### 🔄 Working with GitHub

#### **Creating Repository on GitHub**
1. **Go to GitHub.com**
2. **Click "New repository"**
3. **Fill in repository details**
4. **Choose public or private**
5. **Click "Create repository"**

#### **Connecting Local to GitHub**
```bash
# Add remote origin
git remote add origin https://github.com/username/repository.git

# Push to GitHub
git push -u origin main

# Verify connection
git remote -v
```

#### **Cloning from GitHub**
```bash
# Clone public repository
git clone https://github.com/username/repository.git

# Clone private repository (requires authentication)
git clone https://github.com/username/private-repo.git
```

### 🔐 Authentication Methods

#### **HTTPS Authentication**
```bash
# Username and password (deprecated)
git push https://github.com/username/repository.git

# Personal Access Token
git push https://username:token@github.com/username/repository.git
```

#### **SSH Authentication**
```bash
# Generate SSH key
ssh-keygen -t ed25519 -C "your.email@example.com"

# Add to SSH agent
ssh-add ~/.ssh/id_ed25519

# Add to GitHub
# Copy public key and add to GitHub settings

# Clone with SSH
git clone git@github.com:username/repository.git
```

---

## ❓ Question 8: How to Use Git for Collaboration?

### 👥 Collaboration Workflows

#### **1. Fork and Pull Request (Open Source)**
```bash
# Fork repository on GitHub
# Clone your fork
git clone https://github.com/your-username/repository.git

# Add original repository as upstream
git remote add upstream https://github.com/original-owner/repository.git

# Create feature branch
git checkout -b feature-branch

# Make changes and commit
git add .
git commit -m "Add new feature"

# Push to your fork
git push origin feature-branch

# Create pull request on GitHub
```

#### **2. Shared Repository (Team)**
```bash
# Clone shared repository
git clone https://github.com/team/repository.git

# Create feature branch
git checkout -b feature-branch

# Make changes and commit
git add .
git commit -m "Add new feature"

# Push to shared repository
git push origin feature-branch

# Create pull request on GitHub
```

### 🔄 Pull Request Workflow

#### **Creating Pull Request**
1. **Push your branch to GitHub**
2. **Go to repository on GitHub**
3. **Click "Compare & pull request"**
4. **Fill in description**
5. **Click "Create pull request"**

#### **Reviewing Pull Request**
```bash
# Fetch latest changes
git fetch origin

# Checkout pull request branch
git checkout -b pr-branch origin/feature-branch

# Review changes
git diff main

# Test the changes
# Run tests, check functionality
```

#### **Merging Pull Request**
```bash
# On GitHub:
# 1. Click "Merge pull request"
# 2. Choose merge strategy
# 3. Delete branch

# Locally:
git checkout main
git pull origin main
git branch -d feature-branch
```

### 🔧 Collaboration Best Practices

#### **1. Commit Messages**
```bash
# Good commit messages
git commit -m "feat: Add user authentication"
git commit -m "fix: Resolve login bug"
git commit -m "docs: Update README"

# Bad commit messages
git commit -m "stuff"
git commit -m "wip"
git commit -m "fix"
```

#### **2. Branch Naming**
```bash
# Feature branches
feature/user-authentication
feature/add-payment-gateway

# Bug fix branches
fix/login-error
fix/database-connection

# Hotfix branches
hotfix/security-patch
hotfix/critical-bug
```

#### **3. Pull Request Guidelines**
- **Clear title** describing the change
- **Detailed description** of what was changed
- **Screenshots** for UI changes
- **Test instructions** for reviewers
- **Link to issues** if applicable

### 🔍 Code Review Process

#### **Review Checklist**
- [ ] **Code follows style guidelines**
- [ ] **No obvious bugs**
- [ ] **Tests are included**
- [ ] **Documentation is updated**
- [ ] **Performance is considered**
- [ ] **Security is addressed**

#### **Review Comments**
```bash
# On GitHub:
# 1. Click on specific line
# 2. Add comment
# 3. Submit review

# Respond to comments
# 1. Make requested changes
# 2. Commit and push
# 3. Comment on the review
```

---

## ❓ Question 9: How to Handle Git Conflicts?

### ⚠️ What are Conflicts?

Conflicts occur when **Git cannot automatically merge** changes because the same lines have been modified in different branches.

### 🔍 Identifying Conflicts

#### **During Merge**
```bash
# When merging branches
git merge feature-branch

# Git will show:
# CONFLICT (content): Merge conflict in filename.txt
# Automatic merge failed; fix conflicts and then commit the result.
```

#### **During Pull**
```bash
# When pulling changes
git pull origin main

# Git will show similar conflict message
```

### 🔧 Resolving Conflicts

#### **Step 1: Identify Conflicted Files**
```bash
# Check which files have conflicts
git status

# Output:
# Unmerged paths:
#   (use "git add <file>..." to mark as resolved)
#         both modified: filename.txt
```

#### **Step 2: Open Conflicted Files**
```bash
# Open file in editor
code filename.txt

# You'll see conflict markers:
<<<<<<< HEAD
// Your changes
=======
// Their changes
>>>>>>> feature-branch
```

#### **Step 3: Resolve Conflicts**
```bash
# Edit the file to resolve conflicts
# Remove conflict markers
# Keep the changes you want
# Save the file
```

#### **Step 4: Mark as Resolved**
```bash
# Add resolved file
git add filename.txt

# Commit the resolution
git commit -m "Resolve merge conflict in filename.txt"
```

### 🛠️ Conflict Resolution Strategies

#### **1. Keep Your Changes**
```bash
# In conflicted file, keep your version:
<<<<<<< HEAD
// Your changes
=======
// Their changes
>>>>>>> feature-branch

# Remove markers, keep your changes:
// Your changes
```

#### **2. Keep Their Changes**
```bash
# In conflicted file, keep their version:
<<<<<<< HEAD
// Your changes
=======
// Their changes
>>>>>>> feature-branch

# Remove markers, keep their changes:
// Their changes
```

#### **3. Combine Changes**
```bash
# In conflicted file, combine both:
<<<<<<< HEAD
// Your changes
=======
// Their changes
>>>>>>> feature-branch

# Remove markers, combine:
// Your changes
// Their changes
```

#### **4. Use Git Tools**
```bash
# Use mergetool
git mergetool

# Configure mergetool
git config --global merge.tool vscode
git config --global mergetool.vscode.cmd 'code --wait $MERGED'
```

### 🔄 Advanced Conflict Resolution

#### **Aborting Operations**
```bash
# Abort merge
git merge --abort

# Abort rebase
git rebase --abort

# Abort cherry-pick
git cherry-pick --abort
```

#### **Using Git Log to Understand**
```bash
# See commit history
git log --oneline --graph

# See changes in specific commit
git show commit-hash

# Compare branches
git diff main feature-branch
```

#### **Preventing Conflicts**
```bash
# Always pull before pushing
git pull origin main
git push origin main

# Use feature branches
git checkout -b feature-branch
# Work on feature
git checkout main
git merge feature-branch

# Communicate with team
# Let others know what you're working on
```

---

## ❓ Question 10: How to Use Advanced Git Features?

### 🏷️ Git Tags

#### **Creating Tags**
```bash
# Lightweight tag
git tag v1.0.0

# Annotated tag
git tag -a v1.0.0 -m "Release version 1.0.0"

# Tag specific commit
git tag -a v1.0.0 commit-hash -m "Release version 1.0.0"
```

#### **Managing Tags**
```bash
# List tags
git tag

# Show tag details
git show v1.0.0

# Delete tag
git tag -d v1.0.0

# Push tags to remote
git push origin v1.0.0

# Push all tags
git push origin --tags
```

### 🔍 Git Stash

#### **Stashing Changes**
```bash
# Stash current changes
git stash

# Stash with message
git stash push -m "Work in progress"

# Stash specific files
git stash push filename.txt

# List stashes
git stash list
```

#### **Managing Stashes**
```bash
# Apply latest stash
git stash pop

# Apply specific stash
git stash apply stash@{1}

# Show stash contents
git stash show

# Show stash diff
git stash show -p

# Delete stash
git stash drop stash@{1}

# Delete all stashes
git stash clear
```

### 🔄 Git Rebase

#### **Basic Rebase**
```bash
# Rebase current branch onto main
git rebase main

# Interactive rebase
git rebase -i HEAD~3

# Abort rebase
git rebase --abort

# Continue rebase after resolving conflicts
git rebase --continue
```

#### **Interactive Rebase**
```bash
# Interactive rebase
git rebase -i HEAD~3

# Available commands:
# pick - use commit
# reword - use commit, but edit commit message
# edit - use commit, but stop for amending
# squash - use commit, but meld into previous commit
# fixup - like squash, but discard commit message
# drop - remove commit
```

### 🍒 Git Cherry-pick

#### **Cherry-picking Commits**
```bash
# Cherry-pick single commit
git cherry-pick commit-hash

# Cherry-pick multiple commits
git cherry-pick commit1 commit2 commit3

# Cherry-pick range
git cherry-pick commit1..commit2

# Abort cherry-pick
git cherry-pick --abort
```

### 🔧 Git Submodules

#### **Adding Submodules**
```bash
# Add submodule
git submodule add https://github.com/username/repo.git path/to/submodule

# Initialize submodules
git submodule init

# Update submodules
git submodule update

# Clone repository with submodules
git clone --recursive https://github.com/username/repo.git
```

#### **Managing Submodules**
```bash
# Update submodule to latest
cd path/to/submodule
git pull origin main
cd ..
git add path/to/submodule
git commit -m "Update submodule"

# Remove submodule
git submodule deinit path/to/submodule
git rm path/to/submodule
git commit -m "Remove submodule"
```

### 📊 Git Bisect

#### **Finding Bad Commits**
```bash
# Start bisect
git bisect start

# Mark current commit as bad
git bisect bad

# Mark known good commit
git bisect good commit-hash

# Git will checkout commits for testing
# Mark each as good or bad
git bisect good
git bisect bad

# Reset bisect
git bisect reset
```

### 🎯 Git Hooks

#### **Pre-commit Hook**
```bash
# Create pre-commit hook
cat > .git/hooks/pre-commit << 'EOF'
#!/bin/bash
# Run tests before commit
npm test
if [ $? -ne 0 ]; then
    echo "Tests failed. Commit aborted."
    exit 1
fi
EOF

# Make executable
chmod +x .git/hooks/pre-commit
```

#### **Post-commit Hook**
```bash
# Create post-commit hook
cat > .git/hooks/post-commit << 'EOF'
#!/bin/bash
# Send notification after commit
echo "Commit $(git rev-parse HEAD) created successfully"
EOF

# Make executable
chmod +x .git/hooks/post-commit
```

### 🔍 Git Aliases

#### **Creating Aliases**
```bash
# Create useful aliases
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.unstage 'reset HEAD --'

# Use aliases
git st
git co main
git br feature-branch
git ci -m "Add feature"
git unstage filename.txt
```

#### **Advanced Aliases**
```bash
# Pretty log
git config --global alias.lg "log --oneline --graph --decorate"

# Show last commit
git config --global alias.last "log -1 HEAD"

# Show changes in last commit
git config --global alias.last-diff "diff HEAD~1"

# Show staged changes
git config --global alias.staged "diff --cached"
```

### 📈 Git Worktree

#### **Managing Multiple Worktrees**
```bash
# Add worktree
git worktree add ../hotfix-branch hotfix

# List worktrees
git worktree list

# Remove worktree
git worktree remove hotfix-branch

# Prune worktrees
git worktree prune
```

---

## ❓ Question 11: How to Use GitHub Features?

### 🌐 GitHub Repository Management

#### **Creating Repository**
1. **Go to GitHub.com**
2. **Click "New repository"**
3. **Fill repository details:**
   - Repository name
   - Description
   - Public/Private
   - Initialize with README
   - Add .gitignore
   - Choose license

#### **Repository Settings**
```bash
# Clone repository
git clone https://github.com/username/repository.git

# Add remote
git remote add origin https://github.com/username/repository.git

# Push to GitHub
git push -u origin main
```

### 🔄 Pull Requests

#### **Creating Pull Request**
1. **Push your branch to GitHub**
2. **Click "Compare & pull request"**
3. **Fill in details:**
   - Title
   - Description
   - Assignees
   - Labels
   - Reviewers

#### **Review Process**
```bash
# Fetch pull request locally
git fetch origin pull/123/head:pr-123

# Checkout pull request
git checkout pr-123

# Review changes
git diff main

# Test changes
npm test
```

#### **Merging Pull Request**
- **Merge commit** - Creates merge commit
- **Squash and merge** - Combines all commits
- **Rebase and merge** - Linear history

### 🐛 Issues and Projects

#### **Creating Issues**
1. **Go to repository**
2. **Click "Issues" tab**
3. **Click "New issue"**
4. **Fill in details:**
   - Title
   - Description
   - Labels
   - Assignees
   - Milestone

#### **Issue Templates**
```markdown
## Bug Report

**Description:**
Brief description of the bug

**Steps to reproduce:**
1. Step 1
2. Step 2
3. Step 3

**Expected behavior:**
What should happen

**Actual behavior:**
What actually happens

**Environment:**
- OS: Windows 10
- Browser: Chrome 90
- Version: 1.0.0
```

#### **Projects and Milestones**
- **Projects** - Kanban boards for organizing work
- **Milestones** - Group issues by release or feature
- **Labels** - Categorize issues and pull requests

### 🔧 GitHub Actions

#### **Creating Workflow**
```yaml
# .github/workflows/ci.yml
name: CI

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  test:
    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v2
    
    - name: Use Node.js
      uses: actions/setup-node@v2
      with:
        node-version: '16'
    
    - name: Install dependencies
      run: npm ci
    
    - name: Run tests
      run: npm test
```

#### **Common Actions**
- **CI/CD** - Automated testing and deployment
- **Code quality** - Linting and formatting
- **Security** - Vulnerability scanning
- **Documentation** - Auto-generate docs

### 📚 GitHub Pages

#### **Enabling GitHub Pages**
1. **Go to repository settings**
2. **Scroll to "Pages" section**
3. **Choose source:**
   - Deploy from branch
   - Deploy from actions
4. **Select branch and folder**
5. **Save**

#### **Custom Domain**
```bash
# Add custom domain
# 1. Add CNAME file to repository
echo "yourdomain.com" > CNAME

# 2. Configure DNS
# Add CNAME record pointing to username.github.io
```

### 🔒 Security Features

#### **Branch Protection**
1. **Go to repository settings**
2. **Click "Branches"**
3. **Add rule for main branch:**
   - Require pull request reviews
   - Require status checks
   - Require signed commits
   - Restrict pushes

#### **Security Alerts**
- **Dependabot** - Automated dependency updates
- **Security advisories** - Private security discussions
- **Code scanning** - Automated security analysis

### 📊 GitHub Insights

#### **Repository Analytics**
- **Traffic** - Views and clones
- **Contributors** - Who's contributing
- **Commits** - Activity over time
- **Code frequency** - Lines added/removed

#### **Personal Analytics**
- **Contribution graph** - Your activity
- **Streak** - Consecutive days
- **Repositories** - Your projects

---

## ❓ Question 12: How to Troubleshoot Common Git Issues?

### 🚨 Common Problems and Solutions

#### **1. "Permission Denied" Error**
```bash
# Problem
git push origin main
fatal: Authentication failed

# Solutions:
# 1. Check SSH key
ssh -T git@github.com

# 2. Use personal access token
git remote set-url origin https://username:token@github.com/username/repo.git

# 3. Configure credential helper
git config --global credential.helper store
```

#### **2. "Branch Not Found" Error**
```bash
# Problem
git checkout branch-name
error: pathspec 'branch-name' did not match any file(s) known to git

# Solutions:
# 1. Check available branches
git branch -a

# 2. Fetch from remote
git fetch origin

# 3. Check remote branches
git branch -r
```

#### **3. "Merge Conflict" Error**
```bash
# Problem
git merge feature-branch
CONFLICT (content): Merge conflict in filename.txt

# Solutions:
# 1. Resolve conflicts manually
# Edit conflicted files
# Remove conflict markers
# Add resolved files
git add filename.txt
git commit -m "Resolve merge conflict"

# 2. Abort merge
git merge --abort

# 3. Use merge tool
git mergetool
```

#### **4. "Detached HEAD" State**
```bash
# Problem
git checkout commit-hash
# You are in 'detached HEAD' state

# Solutions:
# 1. Create new branch
git checkout -b new-branch

# 2. Return to main branch
git checkout main

# 3. Reset to main
git reset --hard main
```

#### **5. "Large File" Error**
```bash
# Problem
git push origin main
remote: error: File filename.zip is 100.00 MB; this exceeds GitHub's file size limit

# Solutions:
# 1. Remove large file from history
git filter-branch --force --index-filter \
  'git rm --cached --ignore-unmatch filename.zip' \
  --prune-empty --tag-name-filter cat -- --all

# 2. Use Git LFS
git lfs track "*.zip"
git add .gitattributes
git add filename.zip
git commit -m "Add large file with LFS"
```

### 🔧 Advanced Troubleshooting

#### **Git Log Analysis**
```bash
# Find problematic commit
git log --oneline --graph

# Show commit details
git show commit-hash

# Show file history
git log --follow filename.txt

# Show blame
git blame filename.txt
```

#### **Repository Maintenance**
```bash
# Clean repository
git gc

# Prune unreachable objects
git prune

# Verify repository integrity
git fsck

# Rebuild index
rm .git/index
git reset
```

#### **Recovering Lost Commits**
```bash
# Find lost commits
git reflog

# Recover specific commit
git checkout commit-hash

# Create branch from recovered commit
git checkout -b recovered-branch

# Reset to recovered commit
git reset --hard commit-hash
```

### 🛠️ Performance Issues

#### **Large Repository**
```bash
# Clone with depth limit
git clone --depth 1 https://github.com/username/repo.git

# Shallow clone
git clone --depth 10 https://github.com/username/repo.git

# Clone specific branch only
git clone -b branch-name --single-branch https://github.com/username/repo.git
```

#### **Slow Operations**
```bash
# Use shallow clone for large repos
git clone --depth 1 https://github.com/username/repo.git

# Limit log output
git log --oneline -10

# Use sparse checkout
git sparse-checkout init
git sparse-checkout set folder1 folder2
```

### 🔍 Debugging Commands

#### **Git Debug**
```bash
# Show Git configuration
git config --list

# Show repository information
git remote -v
git branch -a

# Show Git version
git --version

# Show help
git help command-name
```

#### **Network Debug**
```bash
# Test SSH connection
ssh -T git@github.com

# Test HTTPS connection
curl -I https://github.com

# Show network configuration
git config --global --list | grep url
```

---

## 📚 Summary

You've learned:

✅ **What Git and GitHub are** and their purposes
✅ **How to install and configure** Git
✅ **Basic Git commands** for daily use
✅ **Branch management** and workflows
✅ **Remote repository** operations
✅ **Collaboration** techniques
✅ **Conflict resolution** strategies
✅ **Advanced Git features** and tools
✅ **GitHub features** and workflows
✅ **Troubleshooting** common issues

**Congratulations! You now have a comprehensive understanding of Git and GitHub. These skills are essential for modern software development and collaboration.**

---
