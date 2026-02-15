# Costco Passport Website

Marketing website for the Costco Passport iOS app, built with HTML, CSS, and JavaScript. Hosted on GitHub Pages.

## 🌐 Live Site

Visit: [https://gurpreetz.github.io/costco-passport-site/](https://gurpreetz.github.io/costco-passport-site/)

## 📱 About Costco Passport

Costco Passport is an iOS app that helps users track their visits to Costco warehouse locations across America. Users can check in at locations, collect achievements, and explore new states.

## 🚀 Setup

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/costco-passport-site.git
cd costco-passport-site
```

2. Open `index.html` in your browser or use a local server:
```bash
# Using Python 3
python3 -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js
npx http-server
```

3. Visit `http://localhost:8000` in your browser

### GitHub Pages Deployment

1. Push to GitHub:
```bash
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/costco-passport-site.git
git push -u origin main
```

2. Enable GitHub Pages:
   - Go to repository Settings
   - Navigate to Pages section
   - Select "main" branch as source
   - Click Save

3. Your site will be live at: `https://yourusername.github.io/costco-passport-site/`

## 📸 Adding Screenshots

1. Take screenshots in Xcode simulator (iPhone 15 Pro Max recommended)
2. Save screenshots as PNG files
3. Place them in the `screenshots/` directory with these names:
   - `map-view.png` - Main map view
   - `location-detail.png` - Location detail sheet
   - `check-in.png` - Check-in interface
   - `statistics.png` - Statistics dashboard
   - `achievements.png` - Achievements view

4. Recommended dimensions: 1290 x 2796 px (iPhone 15 Pro Max)

## 📁 File Structure

```
costco-passport-site/
├── index.html           # Main landing page
├── styles.css          # All styles
├── script.js           # Interactive features
├── privacy.html        # Privacy policy
├── terms.html          # Terms of service
├── screenshots/        # App screenshots
│   └── README.md       # Screenshot instructions
└── README.md           # This file
```

## 🎨 Customization

### Colors

Edit CSS variables in `styles.css`:

```css
:root {
    --primary-color: #007AFF;
    --primary-dark: #0051D5;
    --secondary-color: #5856D6;
    /* ... */
}
```

### Content

- Update text in `index.html`
- Modify feature descriptions
- Change App Store link when available
- Update contact email

## 🔧 Technologies

- HTML5
- CSS3 (with CSS Grid and Flexbox)
- Vanilla JavaScript
- Google Fonts (Inter)

## 📄 License

This website is independent and not affiliated with Costco Wholesale Corporation.

## 📧 Contact

For questions: gurpreet.appdev@myyahoo.com

---

Built with ❤️ for Costco enthusiasts
