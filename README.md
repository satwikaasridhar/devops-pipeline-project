# devops-pipeline-project
## Project Structure
devops-pipeline-project/
│
├── .gitignore
├── README.md
├── docs/
│   └── task-log.md
├── src/
│   └── ...
├── .github/workflows/
│   └── ci.yml


✅ Step 1: Setup and Initialization
1. Create a GitHub Repository
> Go to GitHub.
> Click on New Repository.
> Name your project (https://github.com/satwikaasridhar/Git_Versions.git).
> Add a description.
> Select Public or Private.
> Do not initialize with README (you'll do it manually).
> Click Create Repository.

2. Clone Repository Locally
bash
Copy
Edit
git clone https://github.com/satwikaasridhar/Git_Versions.git
cd devops-pipeline-project

4. Initialize Git (if not already done)
bash
Copy
Edit
git init

✅ Step 2: Create and Setup Branches
1. Create and Switch to dev Branch
git checkout -b dev

3. Create feature Branch from dev
git checkout -b feature/setup-pipeline
You can later make more feature branches like feature/docker-setup, feature/ci-cd, etc.

✅ Step 3: Add .gitignore and README
1. Add .gitignore
Create a file named .gitignore and add common ignores:
*.log
*.env
__pycache__/
node_modules/
dist/
.DS_Store

2. Add README.md
Create README.md:

# DevOps Pipeline Project

This project demonstrates DevOps CI/CD automation using version control best practices.

## Branch Strategy
- `main` – Stable production-ready code.
- `dev` – Ongoing development.
- `feature/*` – Individual features or tasks.

## Tools Used
- Git
- GitHub
- Docker
- CI/CD Tools (GitHub Actions/Jenkins)

## Getting Started
Steps to clone and run the project locally...\

✅ Step 4: Make Commits
1. Track Changes and Commit
git add .
git commit -m "Initial commit: Added README and .gitignore"

2. Push to GitHub
git push origin feature/setup-pipeline

✅ Step 5: Pull Request & Merge
1. Create Pull Request
> Go to GitHub.
> Create a Pull Request from feature/setup-pipeline → dev.
> Add description and task details.
> Click Create Pull Request.

2. Merge to Dev
After review, click Merge Pull Request → Confirm.

✅ Step 6: Merge to Main
Once stable:
git checkout main
git pull origin main
git merge dev
git push origin main

✅ Step 7: Add Tags (Optional but Good Practice)
git tag -a v1.0 -m "Initial release"
git push origin v1.0
