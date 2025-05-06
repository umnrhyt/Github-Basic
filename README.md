# Panduan Perintah Dasar Git

Panduan ini menjelaskan perintah Git yang paling umum digunakan .

## Perintah Dasar

### 1. Clone a Repository
To download a copy of a repository from GitHub to your computer:
```bash
git clone https://github.com/username/repository-name.git
```
Example:
```bash
git clone https://github.com/username/my-project.git
```

### 2. Check Status
To see what files have been changed and what's staged for commit:
```bash
git status
```
This will show you:
- Files that have been modified
- Files that are staged for commit
- Untracked files

### 3. Add Files
To stage files for commit:
```bash
# Add a specific file
git add filename.txt

# Add all files
git add .
```
Example:
```bash
git add index.html
git add .
```

### 4. Commit Changes
To save your changes with a message:
```bash
git commit -m "Your commit message"
```
Example:
```bash
git commit -m "Added new feature"
```

### 5. Push Changes
To upload your changes to GitHub:
```bash
git push origin main
```
Example:
```bash
git push origin master
```

### 6. Pull Changes
To download and merge changes from GitHub:
```bash
git pull origin main
```
Example:
```bash
git pull origin master
```

### 7. Create and Switch to New Branch
To create and switch to a new branch:
```bash
git checkout -b branch-name
```
Example:
```bash
git checkout -b feature-login
```

### 8. Switch Between Branches
To switch to an existing branch:
```bash
git checkout branch-name
```
Example:
```bash
git checkout main
```

### 9. Stash Changes
To temporarily save your changes without committing:
```bash
# Save changes to stash
git stash

# Apply the most recent stash
git stash pop

# List all stashes
git stash list
```
Example:
```bash
git stash save "WIP: Working on login feature"
```

## Common Workflow Example

1. Clone a repository:
```bash
git clone https://github.com/username/project.git
```

2. Create a new branch for your feature:
```bash
git checkout -b new-feature
```

3. Make changes to files and check status:
```bash
git status
```

4. Add and commit your changes:
```bash
git add .
git commit -m "Added new feature"
```

5. Push your changes:
```bash
git push origin new-feature
```

## Tips
- Always check `git status` before committing
- Write clear commit messages
- Pull changes before starting new work
- Use branches for new features
- Stash changes when you need to switch branches quickly

## Need Help?
If you get stuck, you can always use:
```bash
git help
```
or
```bash
git command --help
```
Replace "command" with any Git command you want to learn more about.
