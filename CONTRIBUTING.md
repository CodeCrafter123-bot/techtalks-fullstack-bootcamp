# Contributing to TechTalks Full-Stack Bootcamp

This guide explains how to submit your assignments to the official TechTalks bootcamp repository.

## Step 1: Set Up Your Student Project Repository

Create your assignment project in a new local folder and push it to its own GitHub repository.

```bash
git init
git add .
git commit -m "Initialize Assignment 1 project"
git branch -M main
git remote add origin https://github.com/USERNAME/REPOSITORY.git
git push -u origin main
```

Replace `USERNAME` with your GitHub username and `REPOSITORY` with your repository name.

## Step 2: Create the Assignment Branch

```bash
git checkout -b assignment-01-firstname-lastname
```

Example:

```bash
git checkout -b assignment-01-khaled-frayji
```

## Step 3: Push the Assignment Work

Complete your assignment on the branch, then push it to GitHub.

```bash
git add .
git commit -m "Complete Assignment 1"
git push -u origin assignment-01-khaled-frayji
```

## Step 4: Open the Student Project Pull Request

Open a pull request in your project repository:

```text
assignment-01-khaled-frayji → main
```

Keep this pull request open for mentor review. Copy the pull request URL because you must include it in your official submission file.

## Step 5: Fork and Clone the Official Repository

Fork the official TechTalks bootcamp repository from GitHub, then clone your fork:

```bash
git clone https://github.com/YOUR_USERNAME/techtalks-fullstack-bootcamp.git
cd techtalks-fullstack-bootcamp
```

## Step 6: Create the Official Submission Branch

```bash
git checkout -b submit-assignment-01-khaled-frayji
```

## Step 7: Create the Submission File

Create a Markdown file under the correct assignment folder using your full name:

```text
submissions/assignment-01/khaled-frayji.md
```

Fill in the submission template with your student information, project links, and description. See the main README for the required template.

## Step 8: Commit the Submission

```bash
git add .
git commit -m "Register Assignment 1 submission - Khaled Frayji"
git push origin submit-assignment-01-khaled-frayji
```

## Step 9: Open the Official Submission Pull Request

Open a pull request from your fork to the official TechTalks repository. Use this title format:

```text
Register Assignment 1 Submission — Khaled Frayji
```

This pull request must contain only your submission Markdown file. Do not include project source code, extra files, or changes to other students' submissions.
