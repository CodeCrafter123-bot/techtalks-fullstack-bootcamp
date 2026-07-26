# Deploying to Vercel

This guide explains how to deploy a Next.js project to Vercel and obtain a production URL for your submission.

## Steps

### 1. Push the Project Repository to GitHub

Make sure your project is pushed to a public GitHub repository before attempting to deploy.

```bash
git push origin main
```

### 2. Sign In to Vercel

Go to [https://vercel.com](https://vercel.com) and sign in using your GitHub account.

### 3. Import the GitHub Repository

1. Click "Add New" and select "Project".
2. Click "Import" next to your assignment repository.

### 4. Configure Environment Variables

If your project requires environment variables:

1. Expand the "Environment Variables" section before deploying.
2. Add each variable name and value.
3. Do not commit `.env` files or secrets to your repository.

### 5. Deploy the Project

Click "Deploy". Vercel will build and deploy your project automatically.

### 6. Copy the Production URL

After the deployment finishes, Vercel will display a production URL. Copy this URL.

The URL format is usually:

```text
https://your-project-name.vercel.app
```

### 7. Test Every Required Route

Open the production URL in a browser and test every route and feature required by the assignment to confirm the deployment works correctly.

### 8. Add the URL to the Official Submission File

Include the production URL in the "Live Deployment" field of your submission Markdown file:

```md
**Live Deployment:** https://your-project-name.vercel.app
```
