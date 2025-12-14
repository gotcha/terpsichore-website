# Quick Start Guide

Your Terpsichore website is ready! Here's what you need to know.

## 📁 What's Inside

```
terpsichore-website/
├── content/                    # Your website content (Markdown)
│   ├── _index.md             # Home page
│   ├── qui-sommes-nous.md    # About Us
│   ├── le-choeur.md          # The Choir
│   ├── le-chef.md            # The Conductor
│   └── nous-rejoindre.md     # Join Us
├── public/                    # Built site (generated)
├── themes/papermod/           # Website theme
├── hugo.toml                  # Configuration
├── .github/workflows/         # GitHub Actions
├── README.md                  # Full documentation
└── DEPLOYMENT.md              # Deployment steps
```

## 🚀 Deploy in 5 Minutes

### 1. Create GitHub Repository
- Go to github.com → Create new repository
- Name: `terpsichore-website`
- Make it Public

### 2. Push Your Code
```bash
cd /Users/gotcha/co/terpsichore-website
git remote add origin https://github.com/YOUR-USERNAME/terpsichore-website.git
git branch -M main
git add .
git commit -m "Initial commit"
git push -u origin main
```

### 3. Enable GitHub Actions
- Go to your repo → Settings → Pages
- Select "GitHub Actions" as source
- Wait for workflow to complete (green checkmark in Actions tab)

### 4. Your Site is Live!
```
https://YOUR-USERNAME.github.io/terpsichore-website/
```

## ✏️ Edit Content

All pages are in French and located in `content/`:

- **Home page**: Edit `content/_index.md`
  - Concert dates, welcome message
  
- **About Us**: Edit `content/qui-sommes-nous.md`
  - Overall about section

- **The Choir**: Edit `content/le-choeur.md`
  - Choir history, repertoire

- **The Conductor**: Edit `content/le-chef.md`
  - Xavier Haag's biography

- **Join Us**: Edit `content/nous-rejoindre.md`
  - How to join instructions

### Make Changes & Deploy
```bash
# 1. Edit a file
nano content/le-choeur.md

# 2. Test locally (optional)
hugo server
# Visit http://localhost:1313

# 3. Commit and push
git add .
git commit -m "Update: [describe what changed]"
git push
```

GitHub Actions will automatically rebuild and deploy your site!

## 🎨 Customize

### Change Site Title
Edit `hugo.toml`:
```toml
title = "Ensemble Vocal Terpsichore"
```

### Update Navigation Menu
Edit `hugo.toml`:
```toml
[[menu.main]]
name = "Your Page Name"
url = "/your-page/"
weight = 5
```

### Add Images
1. Create folder: `static/images/`
2. Add your images
3. Reference in markdown:
```markdown
![Description](/images/your-image.jpg)
```

## 📋 Navigation Menu

The header menu includes:
- Accueil (Home)
- Qui sommes-nous ? (About Us)
- Le choeur (The Choir)
- Le chef (The Conductor)
- Nous rejoindre (Join Us)

All perfectly styled and mobile-responsive!

## 📖 Full Documentation

- **README.md** - Complete project info
- **DEPLOYMENT.md** - Detailed deployment guide
- [Hugo Docs](https://gohugo.io/) - Official Hugo documentation
- [PaperMod Theme](https://github.com/adityatelange/hugo-papermod) - Theme customization

## ⚡ Build & Test Locally

```bash
# Install Hugo (if needed)
# Visit: https://gohugo.io/installation/

# Run development server
cd /Users/gotcha/co/terpsichore-website
hugo server

# Build for production
hugo --minify
# Output in: public/
```

## ✨ Key Features

✅ Beautiful, responsive design  
✅ Fast loading (static HTML)  
✅ SEO friendly  
✅ Mobile-friendly  
✅ Free hosting on GitHub Pages  
✅ Automatic deployments  
✅ All content in French  
✅ Easy to update  

## 🆘 Issues?

### Build failed?
Check `.github/workflows/deploy.yml` output in Actions tab

### Wrong URL?
Update `baseURL` in `hugo.toml` and push again

### Content not showing?
- Make sure file is in `content/` folder
- Check markdown syntax
- Wait 2-5 minutes for deployment

## 📞 Support

- Hugo: https://gohugo.io/
- GitHub Pages: https://docs.github.com/en/pages
- Theme: https://github.com/adityatelange/hugo-papermod

---

**You're all set! Start deploying! 🎉**
