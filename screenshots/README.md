# Screenshots

This folder contains the app screenshots displayed on the website.

## Required Screenshots

Please add the following screenshots to this directory:

### 1. `map-view.png`
- Main map view showing Costco locations
- Show both visited (green) and unvisited (red) pins
- Include the "Center on Me" button
- **Recommended screen**: Map with 5-10 visible locations

### 2. `check-in.png`
- Check-in interface
- Show the favorite items input field
- Display location name and map preview
- **Recommended screen**: Active check-in at a warehouse

### 3. `statistics.png`
- Statistics dashboard
- Show visit counts, states visited
- Display progress percentages
- **Recommended screen**: Statistics with some real data (not empty)

### 4. `achievements.png`
- Achievements view
- Show mix of locked and unlocked achievements
- Include achievement descriptions
- **Recommended screen**: Achievements page with 2-3 unlocked

## Screenshot Guidelines

### Device & Dimensions
- **Device**: iPhone 15 Pro Max (Simulator)
- **Dimensions**: 1290 x 2796 pixels
- **Format**: PNG with transparency support
- **File size**: Keep under 1MB per image

### How to Take Screenshots in Xcode

1. Open your project in Xcode
2. Run the app in iPhone 15 Pro Max simulator
3. Navigate to the screen you want to capture
4. Click the simulator window
5. Press `Cmd + S` or use `File > Save Screen`
6. Save to this directory with the correct filename

### Style Recommendations

**For best presentation:**
- Use light mode for consistency
- Add some visit data so screens aren't empty
- Show realistic usage (visit 3-5 locations first)
- Capture screens during daytime with good visibility
- Ensure UI elements are fully loaded

### Alternative: Command Line

```bash
# Take screenshot of running simulator
xcrun simctl io booted screenshot screenshot-name.png

# Or use simulator menu
# Device > Screenshot in Xcode Simulator
```

## Image Optimization

After capturing screenshots, optionally optimize them:

```bash
# Using ImageOptim (Mac app)
# Drag and drop images

# Or using pngquant (brew install pngquant)
pngquant --quality=80-90 --ext .png --force *.png
```

## Testing Images

After adding screenshots, open `index.html` in a browser to verify they display correctly on the website.

## Current Status

- [ ] map-view.png
- [ ] check-in.png
- [ ] statistics.png
- [ ] achievements.png

---

**Note**: Screenshots are essential for the App Store submission as well, so these will serve double duty!
