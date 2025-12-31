# Programme Evaluation Course Website

A modern, responsive website for the Programme Evaluation course. This website allows students to navigate course materials, view the syllabus, access examples, and explore course content without requiring login.

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

