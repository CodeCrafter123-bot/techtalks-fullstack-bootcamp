# Git and GitHub Guide

This guide explains how to use Git and GitHub throughout the TechTalks Full-Stack Bootcamp submission workflow.

## Creating a GitHub Repository

1. Sign in to GitHub.
2. Click the "+" icon in the top-right corner and select "New repository".
3. Enter your repository name following the required naming format.
4. Set the visibility to Public.
5. Click "Create repository".

## Initializing Git in Your Project

Run the following commands inside your project folder:

```bash
git init
git add .
git commit -m "Initialize project"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

## Adding a Remote

If your local project already exists and you need to connect it to a GitHub repository:

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

## Pushing the Initial Project to Main

```bash
git push -u origin main
```

## Creating Assignment Branches

Create a branch for your assignment work using the required naming format:

```bash
git checkout -b assignment-01-firstname-lastname
```

Example:

```bash
git checkout -b assignment-01-ali-jichi
```

## Opening a Pull Request in Your Student Project

After pushing your assignment branch:

1. Go to your project repository on GitHub.
2. Click "Compare and pull request" or open the "Pull requests" tab.
3. Set the base branch to `main` and the compare branch to your assignment branch.
4. Write a descriptive pull request title following the required format.
5. Click "Create pull request".

This pull request is used for code review by TechTalks mentors.

## Keeping the Review Pull Request Open

Do not merge your code review pull request until the mentor approves it or instructs you to merge it.

Keep the pull request open so that mentors can review your changes, leave comments, and request corrections.

## Responding to Mentor Comments

When a mentor leaves a comment on your pull request:

1. Read the comment carefully.
2. Make the required changes in your local project.
3. Commit and push the changes to the same branch.
4. Respond to the comment on GitHub to let the mentor know the changes have been made.

## Committing Requested Changes

```bash
git add .
git commit -m "Address mentor feedback"
git push origin assignment-01-ali-jichi
```

## Updating the Same Pull Request

Pushing new commits to the same branch automatically updates the open pull request. You do not need to close and reopen it.

## Forking the Official TechTalks Repository

1. Go to the official TechTalks bootcamp repository on GitHub.
2. Click the "Fork" button in the top-right corner.
3. Select your GitHub account as the destination.
4. Clone your fork locally:

```bash
git clone https://github.com/YOUR_USERNAME/techtalks-fullstack-bootcamp.git
cd techtalks-fullstack-bootcamp
```

## Registering a Submission

1. Create a new branch in your fork:

```bash
git checkout -b submit-assignment-01-ali-jichi
```

2. Create your submission Markdown file under the correct assignment folder.
3. Commit and push the file:

```bash
git add .
git commit -m "Register Assignment 1 submission - Ali Jichi"
git push origin submit-assignment-01-ali-jichi
```

## Opening the Official Submission Pull Request

1. Go to your fork of the TechTalks bootcamp repository on GitHub.
2. Click "Compare and pull request".
3. Set the base repository to the official TechTalks repository and the base branch to `main`.
4. Use the required pull request title format.
5. Click "Create pull request".

## Understanding the Two Pull Requests

There are two separate pull requests involved in every submission:

**Pull Request 1 — Student Project Code Review**

- Opened inside your own project repository
- Used for TechTalks mentor code review
- Must remain open until the mentor approves it
- Contains your assignment work

**Pull Request 2 — Official TechTalks Submission Registration**

- Opened from your fork of the official TechTalks bootcamp repository
- Used only to register your submission
- Contains only your submission Markdown file
- Links back to your project repository and code review pull request
