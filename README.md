# Portfolio Website

Personal portfolio website showcasing my projects in computational fluid dynamics, heat transfer, and numerical methods.

## Setup Instructions

### Option 1: GitHub Pages (Recommended)

1. Create a new repository on GitHub (e.g., `portfolio` or `your-username.github.io`)
2. Push these files to the repository
3. Go to Settings → Pages
4. Select source branch: `main` (or `master`)
5. Select folder: `/ (root)`
6. Save

Your site will be available at:
- `https://your-username.github.io/portfolio` (if repo is named `portfolio`)
- `https://your-username.github.io` (if repo is named `your-username.github.io`)

### Option 2: Local Development

1. Open `index.html` in a web browser
2. Or use a local server:
   ```bash
   python -m http.server 8000
   ```
   Then visit `http://localhost:8000`

## Adding New Projects

1. Create a new HTML file in `projects/` directory
2. Add a project card to `index.html` in the projects section
3. Update the project detail page with your project information

## Customization

- Edit `styles.css` to change colors, fonts, and layout
- Update `index.html` to modify content and add more sections
- Add images to `images/` directory and reference them in HTML

## Structure

```
Portfolio/
├── index.html          # Main portfolio page
├── styles.css          # Styling
├── README.md          # This file
├── projects/          # Project detail pages
│   └── cfd.html       # CFD project details
└── images/            # Project images (create as needed)
```

# jonathanvillegas.github.io
