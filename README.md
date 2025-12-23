# Surya Prabhakaran - Portfolio Website

A clean, minimal portfolio website for showcasing architectural and environmental building design projects.

## 📁 File Structure

```
portfolio/
├── index.html              # Main homepage with project grid
├── styles.css             # All styling
├── project-template.html  # Template for individual project pages
├── project1.html         # Individual project pages (create 8 of these)
├── project2.html
├── ...
└── images/
    ├── project1/
    │   ├── cover.jpg      # Thumbnail for homepage grid
    │   ├── image1.jpg     # Full project images (4-6 per project)
    │   ├── image2.jpg
    │   └── ...
    ├── project2/
    │   └── ...
    └── ...
```

## 🚀 Setup Instructions

### 1. **Prepare Your Images**
   - Create a folder structure: `images/project1/`, `images/project2/`, etc.
   - For each project folder, add:
     - `cover.jpg` - The thumbnail image shown on the homepage grid
     - `image1.jpg` through `image6.jpg` - Full project images (4-6 images per project)
   - Recommended image sizes:
     - Cover images: 1200x900px (4:3 ratio)
     - Project detail images: 1600px wide minimum

### 2. **Customize the Homepage (`index.html`)**
   - Update the intro text in the hero section
   - For each of the 8 projects, replace:
     - `<h3>Project Title</h3>` with your actual project name
     - `<p class="project-year">2024</p>` with the correct year
     - `<p class="project-type">Type</p>` with the project category
     - `href="project1.html"` with the correct project page link
     - `src="images/project1/cover.jpg"` with your image path

### 3. **Create Project Pages**
   - Make 8 copies of `project-template.html`
   - Name them: `project1.html`, `project2.html`, ... `project8.html`
   - For each project page, customize:
     - Title and meta tags
     - Project title, year, type, location
     - Project description (2-3 paragraphs)
     - Image paths (4-6 images)
     - Remove unused image tags if you have fewer than 6 images

### 4. **Update Contact Information**
   - In `index.html` and all project pages, update the footer:
     - Replace `your.email@example.com` with your actual email
     - Replace `linkedin.com/in/yourprofile` with your LinkedIn URL

### 5. **Upload to GitHub**
   ```bash
   # Navigate to your local folder
   cd portfolio
   
   # Initialize git (if not already done)
   git init
   
   # Add all files
   git add .
   
   # Commit
   git commit -m "Initial portfolio upload"
   
   # Add your GitHub repository
   git remote add origin https://github.com/yourusername/portfolio.git
   
   # Push to GitHub
   git push -u origin main
   ```

### 6. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Settings → Pages
   - Source: Deploy from a branch
   - Branch: main, folder: / (root)
   - Save
   - Your site will be live at `yourusername.github.io/portfolio`

## 🎨 Customization Tips

### Change Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-bg: #ffffff;      /* Background color */
    --text-primary: #1a1a1a;    /* Main text color */
    --text-secondary: #666666;  /* Secondary text */
    --accent: #2c2c2c;          /* Accent color */
    --border: #e0e0e0;          /* Border color */
    --hover: #f5f5f5;           /* Hover background */
}
```

### Adjust Grid Layout
In `styles.css`, find `.projects-grid`:
```css
grid-template-columns: repeat(auto-fill, minmax(380px, 1fr));
```
- Change `380px` to adjust card width
- For 2 columns: use `repeat(2, 1fr)`
- For 3 columns: use `repeat(3, 1fr)`

### Modify Typography
Change font sizes in `styles.css`:
```css
.hero h1 { font-size: 3rem; }  /* Main heading */
.intro { font-size: 1.25rem; } /* Intro paragraph */
```

## 📝 Project Categories to Consider

Based on your work:
- Building Performance Analysis
- Decarbonization Strategy
- Material Health Assessment
- Climate-Responsive Design
- Daylighting Analysis
- Energy Modeling
- Bio-climatic Design
- Computational Design
- Sustainability Certification (LEED/WELL)
- Passive Design Strategies

## 🔧 Troubleshooting

**Images not showing:**
- Check file paths match your folder structure
- Ensure image filenames match exactly (case-sensitive)
- Verify images are in the correct format (.jpg, .png, .webp)

**Layout looks broken on mobile:**
- The site is responsive by default
- Test on different screen sizes
- Check browser console for errors

**GitHub Pages not updating:**
- Wait 1-2 minutes after pushing changes
- Clear browser cache
- Check GitHub Actions tab for build status

## 📞 Support

For any issues or questions:
- GitHub Issues: Create an issue in your repository
- Documentation: https://pages.github.com/

---

**Created by Claude for Surya Prabhakaran**
