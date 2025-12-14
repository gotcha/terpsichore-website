# 🎶 Terpsichore Website - START HERE

Welcome! Your complete, production-ready website for Ensemble Vocal Terpsichore is ready to deploy.

## ✨ What You Have

A fully functional, modern website built with **Hugo** - a blazing-fast static site generator.

**Features:**
- ✅ 5 pages in French (all content from archived pages)
- ✅ Beautiful, mobile-responsive design
- ✅ Navigation menu with all sections
- ✅ Ready for GitHub Pages (free hosting)
- ✅ Automatic deployment on code changes
- ✅ SEO optimized
- ✅ Super fast loading

## 🚀 Deploy in 3 Steps

### Step 1: Create GitHub Repository (2 minutes)

1. Go to [github.com](https://github.com)
2. Click **+** → **New repository**
3. Name: `terpsichore-website`
4. Choose **Public**
5. Click **Create repository**

### Step 2: Push Your Code (1 minute)

Open terminal and run:

```bash
cd /Users/gotcha/co/terpsichore-website

# Add your GitHub repository
git remote add origin https://github.com/YOUR-USERNAME/terpsichore-website.git

# Push everything
git branch -M main
git add .
git commit -m "Initial commit: Terpsichore website"
git push -u origin main
```

*(Replace `YOUR-USERNAME` with your GitHub username)*

### Step 3: Enable GitHub Pages (1 minute)

1. Go to your repository on GitHub
2. Click **Settings**
3. Click **Pages** (left sidebar)
4. Verify it says "GitHub Actions" as source
5. Done! ✅

## 🌐 Your Site is Live!

**Visit:** `https://YOUR-USERNAME.github.io/terpsichore-website/`

*(Replace with your actual GitHub username)*

The site will be live in 2-5 minutes. GitHub automatically built and deployed it!

## 📄 Pages Included

| Page | URL | Content |
|------|-----|---------|
| Home | `/` | Welcome, concerts, info |
| About Us | `/qui-sommes-nous/` | About the ensemble |
| The Choir | `/le-choeur/` | Choir info & repertoire |
| The Conductor | `/le-chef/` | Xavier Haag biography |
| Join Us | `/nous-rejoindre/` | How to join |

All content is in **French** as extracted from the original website.

## ✏️ Edit Your Website

Everything is in the `content/` folder:

```
content/
├── _index.md              Home page
├── qui-sommes-nous.md     About Us
├── le-choeur.md           The Choir
├── le-chef.md             The Conductor
└── nous-rejoindre.md      Join Us
```

### Make a Quick Edit

Example: Update concert dates

```bash
# Edit the file
nano content/_index.md

# Preview changes locally (optional)
hugo server
# Visit http://localhost:1313

# Save and deploy
git add .
git commit -m "Update concert dates"
git push
```

**That's it!** Your changes deploy automatically in 2-5 minutes.

## 📚 Documentation

| File | Purpose |
|------|---------|
| **QUICKSTART.md** | Quick reference (5-minute overview) |
| **DEPLOYMENT.md** | Detailed deployment instructions |
| **CONTENT_GUIDE.md** | How to edit each page |
| **README.md** | Full project documentation |
| **PROJECT_SUMMARY.txt** | Technical summary |

Start with **QUICKSTART.md** for a quick overview.

## 🎨 Customize Your Site

### Change Site Title

Edit `hugo.toml`:
```toml
title = "Your New Title"
```

### Update Contact Email

Edit `content/nous-rejoindre.md`:
```markdown
**Email** : contact@terpsichore.info
```

### Add Images

1. Create folder: `static/images/`
2. Add your image files
3. Reference in content:
```markdown
![Description](/images/your-image.jpg)
```

## 🔧 Useful Commands

```bash
# Navigate to project
cd /Users/gotcha/co/terpsichore-website

# Preview locally
hugo server

# Build for production
hugo --minify

# Check git status
git status

# Update site
git add .
git commit -m "Your message"
git push
```

## 🆘 Quick Troubleshooting

**Q: My site isn't showing up?**
- A: Check GitHub repository → Actions tab
- Make sure workflow shows green checkmark
- Takes 2-5 minutes to deploy

**Q: How do I update concert dates?**
- A: Edit `content/_index.md`
- Push to GitHub - auto-deploys!

**Q: Can I change the design?**
- A: Yes! Edit `hugo.toml` or check PaperMod theme documentation

**Q: Where do I add images?**
- A: Create `static/images/` folder, add images there

## 📖 Learn More

- [Hugo Documentation](https://gohugo.io/)
- [PaperMod Theme](https://github.com/adityatelange/hugo-papermod)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 🎯 Next Steps

- [ ] Create GitHub repository
- [ ] Push code (3 steps above)
- [ ] Visit your live site
- [ ] Customize with your info
- [ ] Update concert dates
- [ ] Share the link!

## 💡 Tips for Success

1. **Keep content updated** - Especially concert dates
2. **Test locally** - Run `hugo server` before pushing
3. **Use clear commit messages** - Makes history easier to follow
4. **All in French** - Website is French-language
5. **No database needed** - Everything is static HTML

## 🎉 You're Ready!

Everything is set up and tested. All you need to do is:

1. Create the GitHub repository
2. Push your code (3 commands)
3. Wait 2-5 minutes
4. Your site goes live! 🚀

**Questions?** Check DEPLOYMENT.md or QUICKSTART.md

---

**Made with ❤️ using Hugo + GitHub Pages**

*Last updated: December 14, 2024*
