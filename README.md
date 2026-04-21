# PropertyTracker Legal Pages

This repository contains the privacy policy, user agreement, and user guide for the PropertyTracker (储物箱) app.

## Files

- `index.html` - Landing page (Chinese, default)
- `index_en.html` - English landing page
- `privacy.html` / `privacy_zh.html` - Privacy Policy
- `user-agreement.html` / `user-agreement_zh.html` - User Agreement
- `help.html` / `help_zh.html` - User Guide

## Deploy to GitHub Pages

### Option 1: Using GitHub Web Interface

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon (New repository)
3. Repository name: `propertytracker`
4. Make it Public
5. Click **Create repository**

6. In your new repository, click **uploading an existing file**
7. Drag all the HTML files from this folder
8. Click **Commit changes**

8. Go to **Settings** > **Pages**
9. Under "Source", select **Deploy from a branch**
10. Select **main** branch and **/ (root)** folder
11. Click **Save**

12. Wait 1-2 minutes, your site will be live at: `https://loki-21.github.io/propertytracker`

### Option 2: Using Git Command Line

```bash
cd propertytracker-website

# Initialize git repo
git init

# Add all files
git add .

# Commit
git commit -m "Add legal pages for PropertyTracker app"

# Add remote (replace with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/propertytracker.git

# Push to GitHub
git push -u origin main

# Enable GitHub Pages in repository Settings > Pages
```

## Update App Links

After deployment, update the URLs in the app's `SettingsView.swift`:

```swift
Link(destination: URL(string: "https://loki-21.github.io/propertytracker/privacy.html")!) {
Link(destination: URL(string: "https://loki-21.github.io/propertytracker/user-agreement.html")!) {
```

Replace `loki-21` with your GitHub username if different.
