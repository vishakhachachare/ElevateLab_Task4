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

Steps Completed
1. Initialize Repository:
```bash   
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/vishakhachachare/ElevateLab_Task4.git
git push -u origin main

```
2. Create Main, Dev and Feature Branches

- main 

- dev 

- feature

---

3. Pull Requests and Merge

- How to Create a Pull Request on GitHub

- Step 1: Push feature branch
```bash
git checkout feature/readme-update
git push gittask4 feature/readme-update
```

- Step 2: Go to your GitHub repository

Open in your browser:
 https://github.com/vishakhachachare/elevate_lab_task4


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
