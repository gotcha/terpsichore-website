# Ensemble Vocal Terpsichore - Website

A static website for the Ensemble Vocal Terpsichore built with Hugo and deployed on GitHub Pages.

## About

This is the official website for the Ensemble Vocal Terpsichore, a French vocal ensemble directed by Xavier Haag. The site showcases information about the choir, its conductor, upcoming concerts, and how to join.

## Technology Stack

- **Hugo** - Fast static site generator
- **PaperMod Theme** - Clean, minimalist theme
- **GitHub Actions** - Automated deployment
- **GitHub Pages** - Free hosting

## Project Structure

```
terpsichore-website/
├── content/              # Markdown content files
├── themes/papermod/      # Hugo theme
├── static/              # Static files (images, etc.)
├── .github/workflows/   # GitHub Actions workflows
├── hugo.toml            # Hugo configuration
└── README.md            # This file
```

## Content Pages

- **Home** (`_index.md`) - Welcome page with concert information
- **About Us** (`qui-sommes-nous.md`) - Main about page
- **The Choir** (`le-choeur.md`) - Information about the ensemble
- **The Conductor** (`le-chef.md`) - Biography of Xavier Haag
- **Join Us** (`nous-rejoindre.md`) - How to join the ensemble

## Local Development

### Prerequisites

- Hugo (extended version recommended)
- Git

### Installation

1. Clone this repository:
```bash
git clone https://github.com/YOUR-USERNAME/terpsichore-website.git
cd terpsichore-website
```

2. Initialize and update submodules:
```bash
git submodule update --init --recursive
```

3. Run the development server:
```bash
hugo server
```

4. Open your browser to `http://localhost:1313`

### Making Changes

1. Edit markdown files in the `content/` directory
2. Changes will be reflected automatically in the browser
3. Build the site for production:
```bash
hugo --minify
```

## Deployment

### GitHub Pages Setup

1. Push this repository to GitHub
2. Go to repository Settings → Pages
3. Select "Deploy from a branch"
4. Choose branch: `gh-pages`
5. Save

### Automatic Deployment

The GitHub Actions workflow (`.github/workflows/deploy.yml`) will:
1. Build the site whenever you push to `main`
2. Deploy to the `gh-pages` branch automatically
3. GitHub Pages will serve the site at: `https://YOUR-USERNAME.github.io/terpsichore-website/`

### Manual Deployment

To manually deploy:
```bash
hugo --minify
# The `public/` directory contains the built site ready for deployment
```

## Configuration

Edit `hugo.toml` to customize:
- Site title and description
- Base URL (change `your-github-username`)
- Menu items
- Social links
- Theme settings

## Adding Content

To add a new page:

```bash
hugo new content/my-page.md
```

Then edit the markdown file and include front matter:
```yaml
---
title: "Page Title"
---

Your content here...
```

## Customization

### Theme Settings

The PaperMod theme can be customized in `hugo.toml`. Key settings:
- `homeInfoParams` - Home page text
- `defaultTheme` - Light/dark mode
- `socialIcons` - Social media links
- `menu.main` - Navigation menu

### Styling

To customize CSS:
1. Create files in `layouts/` directory
2. Override theme templates as needed

## Support

For questions or contributions:
- Contact: contact@terpsichore.info
- Website: https://www.acj.be/ (Federation)

## License

© Terpsichore 2024 - All rights reserved

## Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [PaperMod Theme](https://github.com/adityatelange/hugo-papermod)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
