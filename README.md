#!/bin/bash

# Set variables
REPO_URL="https://github.com/Adrian-Santander/clinical-risk-stratification-ai.git"
BRANCH="main"
COMMIT_MSG="feat: add full README.md for clinical risk stratification project"

# Ensure we're in the project directory
echo "Starting Git setup for clinical-risk-stratification-ai..."

# 1. Initialize Git if not already
git init

# 2. Add remote if not already set
git remote remove origin 2>/dev/null
git remote add origin $REPO_URL

# 3. Stage README.md
git add README.md

# 4. Commit
git commit -m "$COMMIT_MSG"

# 5. Push to GitHub
git branch -M $BRANCH
git push -u origin $BRANCH

echo "✅ README.md pushed to GitHub successfully!"
