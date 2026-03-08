
# Git Lab 2

## Project Description

This lab demonstrates working with branches, merging, tags, and managing remote branches using Git and GitHub.

---

## Steps With Commands

### 1. Create Local Repository

```
git init
```

---

### 2. Create README File

```
echo "Lab 2 Project" > README.md
git add .
git commit -m "initial commit"
```

---

### 3. Connect Repository to GitHub

```
git remote add origin https://github.com/MariamAli581/Lab2git.git
git branch -M main
git push -u origin main
```

---

### 4. Create dev Branch

```
git checkout -b dev
echo "this file in dev branch" > dev.txt
git add .
git commit -m "add dev file"
git push origin dev
```

---

### 5. Create test Branch

```
git checkout main
git checkout -b test
echo "this file in test branch" > test.txt
git add .
git commit -m "add test file"
git push origin test
```

---

### 6. Merge Branches with main

```
git checkout main
git merge dev
git merge test
git push origin main
```

---

### 7. Delete Branches Locally

```
git branch -d dev
git branch -d test
```

---

### 8. Delete Branches Remotely

```
git push origin --delete dev
git push origin --delete test
```

---

### 9. Create Annotated Tag

```
git tag -a v1.7 -m "version 1.7"
git push origin v1.7
```

---

### 10. List Tags

```
git tag
```

---

### 11. Delete Tag

Local:

```
git tag -d v1.7
```

Remote:

```
git push origin --delete v1.7
```

---

### 12. Add Image to README

<img width="360" height="360" alt="img" src="https://github.com/user-attachments/assets/b9ddc9b2-9e63-4da1-8f6d-e44c5669acea" />

