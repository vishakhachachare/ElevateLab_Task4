# TASK 4: Build a Version-Controlled DevOps Project with Git 

## Objective

Manage a DevOps project using Git best practices, including branching, pull requests, and version control workflows.

---

## Tools Used

Git – Version control

GitHub – Remote repository and collaboration

Markdown – Documentation of workflow and project

---

## Workflow
1. Initialize Git repo
2. Create branches: dev, feature, main
3. Commit changes with descriptive messages
4. Push feature branch
5. Create Pull Request to merge into dev
6. Merge after review
7. Add proper README.md file
8. Use .gitgnore and tags
9. Document all tasks using markdown

---

### Steps Completed
#### 1. Initialize Repository:
```bash   
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/vishakhachachare/ElevateLab_Task4.git
git push -u origin main
```
---

#### 2. Create Main, Dev and Feature Branches

- main 

- dev 

- feature

---

#### 3. Update README.md in Feature Branch
1. Add all workflow details, instructions, or other project documentation.
2. Add a .gitignore file in dev branch to exclude unnecessary files:
 ```bash
node_modules/
.env
*.log
.DS_Store
```
3. Commit changes in dev and feature branch

--- 

#### 4. Pull Requests and Merge

- Case 1: Merge a feature branch into dev:
```bash
# Make sure you are on dev branch
git checkout dev

# Pull latest changes from remote dev branch
git pull origin dev

# Merge feature branch into dev
git merge feature -m "Merge feature into dev"

# Push updated dev branch to GitHub
git push origin dev
```

- Case 2: How to Create a Pull Request on GitHub:

- Step 1: Push feature branch
```bash
git checkout feature
git push origin feature
```

- Step 2: Go to your GitHub repository

   Open in your browser:
  
   https://github.com/vishakhachachare/ElevateLab_Task4


- Step 3: Select the feature branch

   On GitHub, switch the branch dropdown (top-left, above file list) from main to feature.


- Step 4: Click “Compare & pull request”

   GitHub will show a yellow/green bar suggesting that your branch has recent pushes.
  
   Click Compare & pull request.


- Step 5: Choose the target branch

   Base branch (where you want to merge into): dev
  
   Compare branch (feature branch): feature
  
   So it should look like:
   dev ← feature


- Step 6: Add PR details

   Title: Updated README with workflow details
  
   Description: Explain the changes


- Step 7: Create PR

   Click Create pull request.
  
   Now PR is open and visible under the Pull requests tab of your repo.

- Step 8: Merge PR

   Go to the Pull requests tab → open PR.

   Click Merge pull request → Confirm merge.

   This merges feature branch into dev.

---

#### 5. Tagging Versions

```bash
# Create first tag for initial version
git tag v1.0
git tag -a v1.0 -m "Initial version of Task04"

# Create second tag for updated version
git tag v2.0
git tag -a v2.0 -m "Second version of Task04"

# Push tags to GitHub
git push origin --tags

# List tags locally
git tag

# Show details of a specific tag
git show v1.0
```
