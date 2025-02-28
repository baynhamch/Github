# How to Push to GitHub (New and Existing Repos)

Follow these steps to push your Xcode project to GitHub, whether it's a **new repository** or an **existing one**.

---

## **Pushing a New Repository to GitHub**

### 1. **Initialize Git in Your Project**
If your project is not already using Git, initialize it:
```sh
git init
```

### 2. **Add a Remote Repository**
Create a new repository on GitHub, then add it as a remote:
```sh
git remote add origin https://github.com/your-username/your-repo.git
```

### 3. **Add and Commit Your Files**
Stage and commit your initial project files:
```sh
git add .
git commit -m "Initial commit"
```

### 4. **Push to GitHub**
Push your project to GitHub:
```sh
git branch -M main
git push -u origin main
```

Now your project is live on GitHub! 🎉

---

## **Updating an Existing Repository on GitHub**

### 1. **Open Terminal and Navigate to Your Project Folder**
```sh
cd /path/to/your/project
```

### 2. **Check the Status of Your Changes**
Run:
```sh
git status
```
This will show the modified or new files.

### 3. **Stage the Changes**
To add all changes:
```sh
git add .
```
Or add specific files:
```sh
git add filename.swift
```

### 4. **Commit the Changes**
Commit with a message describing the update:
```sh
git commit -m "Updated feature X and fixed bug Y"
```

### 5. **Push to GitHub**
Push the changes to the main branch:
```sh
git push origin main
```
If you're on a different branch (e.g., `dev` or `feature-branch`), replace `main`:
```sh
git push origin your-branch-name
```

### 6. **Verify on GitHub**
Go to your GitHub repository in your browser and confirm the changes are there.

---

## **Troubleshooting**
- **If you get a rejection error**, pull the latest changes first:
  ```sh
  git pull origin main --rebase
  git push origin main
  ```
- **If you get an authentication error**, ensure you're logged into GitHub and using the correct credentials.
- **If pushing a new repository gives an error**, check if you’ve correctly set up the remote repository.


