# GitHub Basics Guide

## Initial Setup

1. **Login to GitHub CLI**
```bash
gh auth login
```

2. **Configure Git (First Time Setup)**
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

## Repository Operations

### Cloning
```bash
# Clone a repository
git clone https://github.com/username/repository.git

# Clone a specific branch
git clone -b branch-name https://github.com/username/repository.git
```

### Basic Commands

1. **Check Status**
```bash
git status
```

2. **Add Files**
```bash
# Add specific file
git add filename.txt

# Add all files
git add .

# Add multiple files
git add file1.txt file2.txt
```

3. **Commit Changes**
```bash
# Commit with message
git commit -m "Your commit message"

# Commit all tracked files
git commit -am "Your commit message"
```

4. **Push Changes**
```bash
# Push to main branch
git push origin main

# Push to different branch
git push origin branch-name

# Push all branches
git push --all
```

## Common Workflows

1. **Update Local Repository**
```bash
# Fetch and merge changes
git pull origin main

# Fetch only
git fetch origin
```

2. **Create and Switch Branches**
```bash
# Create and switch to new branch
git checkout -b new-branch-name

# Switch to existing branch
git checkout branch-name
```

3. **View History**
```bash
# View commit history
git log

# View compact history
git log --oneline
```

## Best Practices

1. **Commit Messages**
- Use clear, descriptive messages
- Start with a verb (Add, Update, Fix, etc.)
- Keep first line under 50 characters
- Add detailed description if needed

2. **Before Pushing**
- Review changes with `git status`
- Check diff with `git diff`
- Ensure tests pass
- Update documentation if needed

3. **Branch Management**
- Keep main/master branch stable
- Create feature branches for new work
- Delete merged branches

## Troubleshooting

1. **Undo Last Commit**
```bash
# Undo commit but keep changes
git reset --soft HEAD~1

# Undo commit and discard changes
git reset --hard HEAD~1
```

2. **Discard Changes**
```bash
# Discard changes in specific file
git checkout -- filename

# Discard all changes
git checkout -- .
```
