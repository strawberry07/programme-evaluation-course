# Programme Evaluation Course Website

A modern, responsive website for the Programme Evaluation course. This website allows students to navigate course materials, view the syllabus, access examples, and explore course content without requiring login.

## 🌐 Publishing on GitHub Pages

This website is ready to be published on GitHub Pages. Follow these steps:

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right → "New repository"
3. Name your repository (e.g., `programme-evaluation-course`)
4. **Do NOT** initialize with README, .gitignore, or license (we already have these)
5. Click "Create repository"

### Step 2: Push Your Code to GitHub

Run these commands in your terminal (from the project directory):

```bash
cd /Users/jessicali/programme-evaluation-course

# Add the GitHub remote (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

### Step 4: Access Your Website

Your website is now live at:
```
https://strawberry07.github.io/programme-evaluation-course/
```

**Note:** It may take a few minutes for the site to be live after enabling Pages.

### Step 5: Set Up Custom Domain (Optional)

If you want to use a custom domain (e.g., `course.yourdomain.com`):

1. **Edit the CNAME file:**
   - Open `CNAME` in this repository
   - Replace the content with your domain name (e.g., `course.yourdomain.com`)
   - No `http://` or `https://`, just the domain name
   - Commit and push the change

2. **Configure DNS with your domain provider:**
   - Add a CNAME record pointing to: `strawberry07.github.io`
   - Or add A records pointing to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`

3. **Enable custom domain in GitHub:**
   - Go to repository Settings → Pages
   - Under "Custom domain", enter your domain
   - Check "Enforce HTTPS" (recommended)

**Note:** DNS changes can take 24-48 hours to propagate.

### Updating Your Website

After making changes to your files:

```bash
git add .
git commit -m "Update website content"
git push
```

Changes will be automatically reflected on your GitHub Pages site (may take 1-2 minutes).

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Navigation**: Easy-to-use navigation menu with smooth scrolling
- **Course Outline**: Comprehensive overview of course modules and learning objectives
- **Syllabus**: Detailed course information including schedule, assessment, and requirements
- **Materials Section**: Organized access to textbooks, readings, slides, and resources
- **Examples & Case Studies**: Showcase of real-world evaluation examples

## Getting Started

### Viewing the Website

1. Simply open `index.html` in your web browser
2. No server or build process required - it's a static website

### Local Development

If you want to serve it locally (optional):

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Then open http://localhost:8000 in your browser
```

## Customizing Content

### Updating Course Outline

Edit the Course Outline section in `index.html`:
- Modify the learning objectives in the `<ul class="objectives-list">` section
- Update or add course modules in the `.modules-grid` section

### Updating Syllabus

Edit the Syllabus section in `index.html`:
- Update course information in the `.syllabus-info` section
- Modify the weekly schedule in the `.schedule-table` section
- Adjust assessment percentages in the `.assessment-grid` section

### Adding Materials

Add your course materials to the Materials section:
- Update the `.material-list` items in each `.material-card`
- Add links to actual files or resources as needed

### Adding Examples

Add your examples and case studies:
- Update the `.example-card` elements in the Examples section
- Add actual links to PDFs, documents, or other resources
- Modify the tags and descriptions as needed

## File Structure

```
programme-evaluation-course/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # JavaScript for interactivity
└── README.md          # This file
```

## Styling

The website uses CSS custom properties (variables) for easy theming. You can customize colors by modifying the `:root` variables in `styles.css`:

```css
:root {
    --primary-color: #2563eb;
    --primary-dark: #1e40af;
    --secondary-color: #64748b;
    /* ... etc */
}
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Notes

- This is a static website - no backend or database required
- All content is editable directly in the HTML file
- Images and additional resources can be added to a `assets/` folder if needed
- The website uses modern CSS features (Grid, Flexbox, CSS Variables)

## License

This website template is provided for educational use.

