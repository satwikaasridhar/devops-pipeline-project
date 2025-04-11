# Devops-pipeline-project

✅ **Step 1: Setup and Initialization**
1. Create a GitHub Repository
2. Go to GitHub.
3. Click on New Repository.
4. Name your project (https://github.com/satwikaasridhar/Git_Versions.git).
5. Add a description.
6. Select Public or Private.
7. Do not initialize with README.
8. Click Create Repository.

2. `Clone Repository Locally`
git clone https://github.com/satwikaasridhar/Git_Versions.git
cd devops-pipeline-project

4. `Initialize Git`
git init

✅ **Step 2: Create and Setup Branches**
1. `Create and Switch to dev Branch`
git checkout -b dev

2. `Create feature Branch from dev`
git checkout -b feature/setup-pipeline
You can later make more feature branches like feature/docker-setup, feature/ci-cd, etc.

✅ **Step 3: Add .gitignore and README**
1. `Add .gitignore`
Create a file named .gitignore and add common ignores:
*.log
*.env
__pycache__/
node_modules/
dist/
.DS_Store

2. *Add README.md*
Create README.md:

# DevOps Pipeline Project

This project demonstrates DevOps CI/CD automation using version control best practices.

## Branch Strategy
- `main` – Stable production-ready code.
- `dev` – Ongoing development.
- `feature/*` – Individual features or tasks.

## Tools Used
- Git
- GitHub Actions

## Getting Started
Steps to clone and run the project locally...\

✅ **Step 4: Make Commits**
1. `Track Changes and Commit`
git add .
git commit -m "Initial commit: Added README and .gitignore"

2. `Push to GitHub`
git push origin feature/setup-pipeline

✅ **Step 5: Pull Request & Merge**
`Create Pull Request`
1. Go to GitHub.
2. Create a Pull Request from feature/setup-pipeline → dev.
3. Add description and task details.
4. Click Create Pull Request.

`Merge to Dev`
After review, click Merge Pull Request → Confirm.

✅ **Step 6: Merge to Main**
*Once stable:*
git checkout main
git pull origin main
git merge dev
git push origin main

✅ **Step 7: Add Tags**
git tag -a v1.0 -m "Initial release"
git push origin v1.0

![Screenshot (42)](https://github.com/user-attachments/assets/ad055eb8-3d3a-4896-a379-2ba9e5f1c84b)

![Screenshot (43)](https://github.com/user-attachments/assets/b19243a7-7ad5-4b36-aba1-57167bb48558)

![Screenshot (44)](https://github.com/user-attachments/assets/bcf7c727-ec66-4e3d-8a99-7eb01ef91b60)

![Screenshot (45)](https://github.com/user-attachments/assets/155e91bd-e375-4c3f-8d54-346ab8ae0ab4)

![Screenshot (46)](https://github.com/user-attachments/assets/e758b3d0-1e83-4b67-8f6d-844d05e51ac2)




