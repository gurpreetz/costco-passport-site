# Website Launch Checklist

Use this checklist to track your progress in launching the Costco Passport website.

## 📸 Screenshots (Do This First!)

Before deploying, take these screenshots in Xcode:

- [ ] **Map View** - Main map with pins (mix of visited/unvisited)
- [ ] **Location Detail** - Detail sheet for a warehouse
- [ ] **Check-In** - Check-in screen with favorite items
- [ ] **Statistics** - Stats dashboard with data
- [ ] **Achievements** - Achievements view (some unlocked)

**Tips:**
- Run app in iPhone 15 Pro Max simulator
- Add 3-5 check-ins first so screens have data
- Save screenshots: Cmd+S in simulator
- Save to `/Users/gps/src/costco-passport-site/screenshots/`
- Use exact filenames listed in `screenshots/README.md`

## 🚀 Deployment

- [ ] Create new repository on GitHub
  - Name: `costco-passport-site`
  - Visibility: Public
  - Don't initialize with README
  
- [ ] Push code to GitHub
  ```bash
  git remote add origin https://github.com/YOUR_USERNAME/costco-passport-site.git
  git push -u origin main
  ```

- [ ] Enable GitHub Pages
  - Go to Settings → Pages
  - Source: main branch, / (root)
  - Save and wait 1-2 minutes

- [ ] Verify site is live
  - Visit: `https://YOUR_USERNAME.github.io/costco-passport-site/`
  - Test all navigation links
  - Check mobile responsiveness

## 📝 Pre-Launch Updates

- [ ] Update contact email in:
  - `index.html` (footer section)
  - `privacy.html`
  - `terms.html`

- [ ] Add screenshots (if not done already)
  ```bash
  git add screenshots/*.png
  git commit -m "Add app screenshots"
  git push
  ```

- [ ] Test all pages:
  - [ ] Home page loads correctly
  - [ ] Features section displays
  - [ ] Screenshots show (or placeholders visible)
  - [ ] Privacy policy accessible
  - [ ] Terms of service accessible
  - [ ] Footer links work

## 🎨 Optional Customization

- [ ] Add custom favicon (app icon)
- [ ] Set up custom domain (if purchased)
- [ ] Add Google Analytics tracking
- [ ] Add Open Graph meta tags for social sharing
- [ ] Create social media graphics using screenshots

## 📱 After App Store Approval

- [ ] Update App Store link in `index.html`
  - Replace `#` in download buttons with actual App Store URL
  
- [ ] Add App Store badge image
  
- [ ] Update README with live URLs

- [ ] Share website on:
  - [ ] App Store listing
  - [ ] Social media
  - [ ] Main app repository README
  - [ ] Personal website/portfolio

## 🔗 Integration with Main Repo

- [ ] Add website link to main app README
  ```markdown
  ## 🌐 Website
  Visit [costcopassport.app](https://YOUR_USERNAME.github.io/costco-passport-site/)
  ```

- [ ] Link to privacy policy and terms in app (if needed)

## 📊 Post-Launch

- [ ] Monitor Google Analytics (if added)
- [ ] Check for broken links
- [ ] Test on multiple devices
- [ ] Gather user feedback
- [ ] Update content based on feedback

---

## Quick Commands Reference

```bash
# Navigate to site directory
cd /Users/gps/src/costco-passport-site

# Make updates
git add .
git commit -m "Your update description"
git push

# View current status
git status

# See commit history
git log --oneline
```

---

**Current Status:** ✅ Website created, ready for screenshots and deployment!

**Next Step:** Take app screenshots in Xcode simulator
