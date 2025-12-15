# Mustafizur Rahaman - Portfolio Website

A professional portfolio website showcasing research, publications, projects, and experience in Geographic Information Science, Deep Learning, and Remote Sensing.

## 🌟 Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean white and light green color scheme with smooth animations
- **Single Page Application**: Easy navigation with smooth scrolling
- **Interactive Elements**: Hover effects, fade-in animations, and dynamic content
- **Professional Sections**:
  - Hero section with contact links
  - About section with research interests
  - Education timeline
  - Publications showcase
  - Experience timeline
  - Featured projects
  - Technical skills
  - Contact information and references

## 🚀 Quick Start - Deploy to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and log in to your account
2. Click the **"+"** icon in the top right corner and select **"New repository"**
3. Name your repository (choose one):
   - For personal site: `yourusername.github.io` (recommended)
   - For project site: `portfolio` or any name you prefer
4. Set the repository to **Public**
5. Click **"Create repository"**

### Step 2: Upload Files to GitHub

You have two options:

#### Option A: Using GitHub Web Interface (Easier)

1. In your new repository, click **"uploading an existing file"**
2. Drag and drop ALL the files from the portfolio folder:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md`
   - `assets/` folder (with CV.pdf inside)
3. Scroll down and click **"Commit changes"**

#### Option B: Using Git Command Line (Recommended)

1. Open your terminal/command prompt
2. Navigate to the portfolio folder
3. Run these commands:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository as remote
# Replace 'yourusername' and 'repository-name' with your actual values
git remote add origin https://github.com/yourusername/repository-name.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** in the left sidebar
4. Under **"Source"**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **"Save"**

### Step 4: Access Your Live Website

Your website will be live in a few minutes at:
- Personal site: `https://yourusername.github.io/`
- Project site: `https://yourusername.github.io/repository-name/`

## 📝 Customization Guide

### Update Contact Information

Edit `index.html` and search for these sections to update:

1. **Email**: Line ~23 (navbar), Line ~372 (contact section)
2. **Phone**: Line ~373
3. **GitHub**: Line ~24, ~374
4. **Google Sites**: Line ~25, ~375
5. **Social Links**: Lines ~40-44

### Update CV

1. Replace `assets/CV.pdf` with your updated CV
2. Make sure the filename remains `CV.pdf` or update the link in `index.html` (line ~38)

### Update Content

- **About Me**: Lines ~58-75 in `index.html`
- **Research Interests**: Lines ~76-86
- **Education**: Lines ~95-120
- **Publications**: Lines ~128-205
- **Experience**: Lines ~214-300
- **Projects**: Lines ~309-370
- **Skills**: Lines ~379-420

### Change Colors

Edit `styles.css` and modify the CSS variables at the top:

```css
:root {
    --primary-green: #2ecc71;      /* Main green color */
    --light-green: #a8e6cf;        /* Light green accents */
    --dark-green: #27ae60;         /* Dark green for hover */
    --very-light-green: #e8f8f5;   /* Very light green background */
    /* ... other colors ... */
}
```

## 🛠️ Technology Stack

- **HTML5**: Structure and content
- **CSS3**: Styling with modern features (Grid, Flexbox, Animations)
- **JavaScript**: Interactive functionality and dynamic effects
- **Font Awesome**: Icons
- **GitHub Pages**: Free hosting

## 📱 Browser Compatibility

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📂 File Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
├── README.md           # This file
└── assets/
    └── CV.pdf         # Your CV/Resume
```

## 🎨 Color Scheme

- **Primary Green**: #2ecc71
- **Light Green**: #a8e6cf
- **Dark Green**: #27ae60
- **Very Light Green**: #e8f8f5
- **White**: #ffffff
- **Text Color**: #333333

## ✨ Key Features Explained

### Responsive Navigation
- Desktop: Horizontal menu
- Mobile: Hamburger menu with smooth transitions

### Smooth Scrolling
- Click any navigation link for smooth scroll to section
- Automatic active section highlighting

### Animations
- Fade-in effects on scroll
- Hover animations on cards
- Typing effect on hero subtitle
- Smooth page transitions

### Interactive Elements
- Scroll-to-top button (appears after scrolling down)
- Hide navbar on scroll down, show on scroll up
- Card hover effects with elevation changes

## 🔧 Maintenance

### Adding New Publications

1. Open `index.html`
2. Find the Publications section (around line 128)
3. Copy an existing publication card
4. Update the content (title, authors, venue, DOI link)

### Adding New Projects

1. Open `index.html`
2. Find the Projects section (around line 309)
3. Copy an existing project card
4. Update content and GitHub link

### Updating Experience

1. Open `index.html`
2. Find the Experience section (around line 214)
3. Add new experience items following the existing structure

## 📞 Support

If you encounter any issues:

1. Check that all files are uploaded correctly
2. Verify GitHub Pages is enabled in repository settings
3. Clear browser cache and hard reload (Ctrl+Shift+R or Cmd+Shift+R)
4. Wait a few minutes after enabling GitHub Pages

## 📄 License

This portfolio template is free to use and modify for personal purposes.

---

**Built with ❤️ by Mustafizur Rahaman**

Last Updated: December 2024
