# GitHub Pages Deployment Instructions

This guide will help you deploy the Costco Passport website to GitHub Pages.

## Prerequisites

- GitHub account
- Git installed on your computer
- The website files in `/Users/gps/src/costco-passport-site/`

## Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com/new)
2. Repository name: `costco-passport-site` (or any name you prefer)
3. Description: "Marketing website for Costco Passport iOS app"
4. Set to **Public** (required for free GitHub Pages)
5. **Don't** initialize with README (we already have one)
6. Click "Create repository"

## Step 2: Push to GitHub

Run these commands in your terminal:

```bash
cd /Users/gps/src/costco-passport-site

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: Costco Passport website"

# Add your GitHub remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/costco-passport-site.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under "Source":
   - Branch: Select `main`
   - Folder: Select `/ (root)`
5. Click **Save**

## Step 4: Wait for Deployment

- GitHub will build and deploy your site (takes 1-2 minutes)
- You'll see a green checkmark when it's ready
- Your site URL will be: `https://YOUR_USERNAME.github.io/costco-passport-site/`

## Step 5: Add Screenshots

Before the site looks complete, add your app screenshots:

```bash
# After taking screenshots in Xcode
cd /Users/gps/src/costco-passport-site/screenshots

# Copy your screenshots here (rename them to match):
# - map-view.png
# - location-detail.png
# - check-in.png
# - statistics.png
# - achievements.png

# Commit and push
git add screenshots/*.png
git commit -m "Add app screenshots"
git push
```

GitHub Pages will automatically redeploy with your new screenshots!

## Custom Domain (Optional)

To use a custom domain like `costcopassport.app`:

1. Buy domain from registrar (Namecheap, Google Domains, etc.)
2. Add a file named `CNAME` in the root with your domain:
   ```
   costcopassport.app
   ```
3. Configure DNS records at your registrar:
   - Type: `A` 
   - Name: `@`
   - Value: `185.199.108.153`
   - Add 3 more A records with: `.109.153`, `.110.153`, `.111.153`
   
4. Or for subdomain (www):
   - Type: `CNAME`
   - Name: `www`
   - Value: `YOUR_USERNAME.github.io`

5. In GitHub Settings → Pages, add your custom domain

## Updating the Site

To make changes:

```bash
cd /Users/gps/src/costco-passport-site

# Edit your files (index.html, styles.css, etc.)

# Commit changes
git add .
git commit -m "Description of changes"
git push

# GitHub Pages automatically deploys in ~1 minute
```

## Troubleshooting

### Site Not Loading
- Check if GitHub Pages is enabled in Settings
- Verify branch is set to `main` and folder to `/root`
- Wait a few minutes for initial deployment

### 404 Error
- Ensure `index.html` is in the root directory
- Check file names are lowercase
- Clear browser cache

### Images Not Showing
- Verify image paths in HTML (should be relative: `screenshots/map-view.png`)
- Check images are committed and pushed to GitHub
- Ensure image files are PNG format

### CSS Not Loading
- Check `styles.css` is in root directory
- Verify link in HTML: `<link rel="stylesheet" href="styles.css">`
- Clear browser cache and hard reload (Cmd+Shift+R)

## Success!

Your website should now be live at:
```
https://YOUR_USERNAME.github.io/costco-passport-site/
```

Share this URL on:
- App Store listing
- Social media
- README in main app repo

---

**Next Steps:**
1. Take and add app screenshots
2. Update the App Store link when app is published
3. Set up Google Analytics (optional)
4. Add Open Graph meta tags for social sharing
