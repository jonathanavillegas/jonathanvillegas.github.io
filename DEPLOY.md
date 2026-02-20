# GitHub Pages Deployment Instructions

## Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. Repository name: `portfolio` (or `jonathanvillegas.github.io` for user site)
3. Make it **Public**
4. **DO NOT** check "Add a README file"
5. Click "Create repository"

## Step 2: Push Files to GitHub

Run these commands in your terminal:

```bash
cd /Users/jonathanvillegas/Code/Portfolio

# Initialize git repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial portfolio commit"

# Rename branch to main (if needed)
git branch -M main

# Add your GitHub repository as remote
# REPLACE 'your-username' with your actual GitHub username
git remote add origin https://github.com/your-username/portfolio.git

# Push to GitHub
git push -u origin main
```

**Note:** Replace `your-username` with your actual GitHub username in the remote URL.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub: `https://github.com/your-username/portfolio`
2. Click **Settings** (top right of repository page)
3. Scroll down to **Pages** in the left sidebar
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

## Step 4: Access Your Site

After a few minutes, your site will be available at:
- `https://your-username.github.io/portfolio` (if repo is named `portfolio`)
- OR `https://your-username.github.io` (if repo is `your-username.github.io`)

**Note:** It may take 1-5 minutes for GitHub Pages to build and deploy your site.

## Troubleshooting

- If you see a 404, wait a few minutes and refresh
- Check that all files are in the repository
- Make sure the branch is `main` (not `master`)
- Verify GitHub Pages is enabled in Settings → Pages


