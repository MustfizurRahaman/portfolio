# 🚀 Step-by-Step Deployment Guide

This guide will walk you through deploying your portfolio website to GitHub Pages, even if you've never used GitHub before!

## Prerequisites

- A GitHub account (free) - [Sign up here](https://github.com/join) if you don't have one
- Your portfolio files (you already have these!)

---

## Method 1: GitHub Web Interface (No Command Line Needed!)

### Step 1: Create a New Repository

1. **Log in to GitHub** at [github.com](https://github.com)

2. **Click the "+" icon** in the top-right corner of the page

3. **Select "New repository"**

4. **Configure your repository:**
   - **Repository name**: Choose one option:
     - For personal portfolio: `YourUsername.github.io` (e.g., `mustafizurrahaman.github.io`)
       - ✅ This will be accessible at: `https://yourusername.github.io`
     - For project portfolio: `portfolio` or any name
       - ✅ This will be accessible at: `https://yourusername.github.io/portfolio`
   
   - **Description** (optional): "Personal Portfolio Website"
   
   - **Public**: ✅ Select this (required for free GitHub Pages)
   
   - **Initialize repository**: ⬜ Leave all checkboxes unchecked

5. **Click "Create repository"**

### Step 2: Upload Your Files

1. **In your new repository**, you'll see a setup page. Click the link that says **"uploading an existing file"**

2. **Upload all your portfolio files**:
   - Drag and drop these files from your portfolio folder:
     - `index.html`
     - `styles.css`
     - `script.js`
     - `README.md`
     - `.gitignore`
   
3. **Upload the assets folder**:
   - Click "uploading an existing file" again
   - Navigate to the `assets` folder and upload `CV.pdf`
   - You can also upload the entire `assets` folder at once

4. **Commit the files**:
   - Scroll down to the "Commit changes" section
   - Add a commit message: "Initial portfolio upload"
   - Click **"Commit changes"**

### Step 3: Enable GitHub Pages

1. **Go to Settings**:
   - Click the **"Settings"** tab at the top of your repository

2. **Navigate to Pages**:
   - In the left sidebar, scroll down and click **"Pages"**

3. **Configure GitHub Pages**:
   - Under "Source":
     - Branch: Select **"main"** (or "master")
     - Folder: Select **"/ (root)"**
   - Click **"Save"**

4. **Wait for deployment**:
   - GitHub will show a message: "Your site is ready to be published at..."
   - Wait 1-2 minutes for the deployment to complete

5. **Visit your website**:
   - Refresh the Settings > Pages page
   - You'll see: "Your site is live at https://yourusername.github.io/"
   - Click the link to view your portfolio! 🎉

---

## Method 2: Using Git Command Line (For Advanced Users)

### Step 1: Install Git

**Windows:**
- Download from [git-scm.com](https://git-scm.com/download/win)
- Run the installer with default settings

**Mac:**
- Open Terminal
- Run: `git --version` (will prompt to install if not present)
- Or install via Homebrew: `brew install git`

**Linux:**
```bash
# Ubuntu/Debian
sudo apt-get install git

# Fedora
sudo dnf install git
```

### Step 2: Configure Git (First Time Only)

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 3: Create Repository on GitHub

1. Go to [github.com](https://github.com)
2. Click "+" → "New repository"
3. Name it `yourusername.github.io` or `portfolio`
4. Click "Create repository"
5. **Keep this page open** - you'll need the repository URL

### Step 4: Deploy from Terminal

```bash
# Navigate to your portfolio folder
cd /path/to/portfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit: Deploy portfolio website"

# Add your GitHub repository as remote
# Replace with YOUR repository URL from Step 3
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

### Step 5: Enable GitHub Pages

Follow the same steps as Method 1, Step 3.

---

## 🔧 Updating Your Portfolio

### Using Web Interface:

1. Go to your repository on GitHub
2. Click on the file you want to edit (e.g., `index.html`)
3. Click the pencil icon (✏️) to edit
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes for changes to appear on your site

### Using Git:

```bash
# Make your changes to the files

# Add the changed files
git add .

# Commit with a descriptive message
git commit -m "Updated projects section"

# Push to GitHub
git push
```

---

## 🌐 Using a Custom Domain (Optional)

### Step 1: Purchase a Domain
- Buy from: [Namecheap](https://www.namecheap.com), [Google Domains](https://domains.google), [GoDaddy](https://www.godaddy.com), etc.

### Step 2: Configure DNS Settings

Add these DNS records in your domain provider's settings:

```
Type    Name    Value
A       @       185.199.108.153
A       @       185.199.109.153
A       @       185.199.110.153
A       @       185.199.111.153
CNAME   www     yourusername.github.io
```

### Step 3: Add CNAME File

1. In your repository, create a new file named `CNAME` (no extension)
2. Add your domain (e.g., `www.yourdomain.com`)
3. Commit the file

### Step 4: Configure in GitHub

1. Go to Settings > Pages
2. Under "Custom domain", enter your domain
3. Click "Save"
4. Wait 24-48 hours for DNS propagation

---

## ✅ Verification Checklist

After deployment, check:

- [ ] Website is accessible at the GitHub Pages URL
- [ ] All sections load correctly
- [ ] Navigation links work
- [ ] CV download works
- [ ] External links (GitHub, email, etc.) work
- [ ] Website is responsive on mobile
- [ ] All images/icons load properly

---

## 🐛 Troubleshooting

### Issue: "404 - Page Not Found"

**Solution:**
- Make sure your `index.html` file is in the root directory (not in a subfolder)
- Check that GitHub Pages is enabled in Settings > Pages
- Wait a few minutes after enabling GitHub Pages

### Issue: "Site shows old content"

**Solution:**
- Clear your browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Wait 5 minutes for GitHub to build the new version
- Check the Actions tab to see if the build is in progress

### Issue: "CSS/JS not loading"

**Solution:**
- Verify that `styles.css` and `script.js` are in the same folder as `index.html`
- Check file names are exactly: `styles.css` and `script.js` (case-sensitive)
- Check browser console (F12) for error messages

### Issue: "CV download doesn't work"

**Solution:**
- Make sure `CV.pdf` is in the `assets` folder
- Verify the file was uploaded to GitHub
- Check the link in `index.html` points to `assets/CV.pdf`

### Issue: "Changes not showing up"

**Solution:**
- Commit and push your changes
- Wait 1-2 minutes for deployment
- Hard refresh your browser (Ctrl+Shift+R)
- Check GitHub Actions tab for build status

---

## 📞 Need More Help?

- **GitHub Pages Documentation**: [docs.github.com/pages](https://docs.github.com/en/pages)
- **GitHub Community**: [github.community](https://github.community)
- **Video Tutorials**: Search YouTube for "GitHub Pages tutorial"

---

## 🎉 Success!

Once deployed, share your portfolio:
- Add the link to your resume
- Share on LinkedIn
- Include in email signatures
- Add to your GitHub profile README

**Your portfolio URL:**
```
https://yourusername.github.io
```

**Congratulations on deploying your portfolio! 🚀**

---

*Last Updated: December 2024*
