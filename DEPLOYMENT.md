# Deployment Guide - GitHub Pages

This guide walks you through deploying the Terpsichore website to GitHub Pages.

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and log in
2. Click the "+" icon → "New repository"
3. Name it: `terpsichore-website`
4. Add description: "Website for Ensemble Vocal Terpsichore"
5. Choose "Public" (so it's accessible)
6. Click "Create repository"

## Step 2: Push Your Code

In your terminal, from the `terpsichore-website` directory:

```bash
# Add the remote repository
git remote add origin https://github.com/YOUR-USERNAME/terpsichore-website.git

# Create and switch to main branch
git branch -M main

# Add all files
git add .

# Commit your changes
git commit -m "Initial commit: Terpsichore website with Hugo"

# Push to GitHub
git push -u origin main
```

## Step 3: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" (top right)
3. Click "Pages" in the left sidebar
4. Under "Build and deployment":
   - Select "GitHub Actions" as the source
5. The workflow will automatically run

## Step 4: Enable GitHub Actions

1. In your repository, click "Actions" tab
2. You should see the "Deploy to GitHub Pages" workflow
3. It will automatically run on each push to `main`
4. Wait for it to complete (green checkmark)

## Step 5: Access Your Site

Your website will be available at:
```
https://YOUR-USERNAME.github.io/terpsichore-website/
```

(Replace `YOUR-USERNAME` with your GitHub username)

## Step 6: Update Configuration

Edit `hugo.toml` and update:

```toml
baseURL = "https://YOUR-USERNAME.github.io/terpsichore-website/"
```

Then commit and push:
```bash
git add hugo.toml
git commit -m "Update baseURL for GitHub Pages"
git push
```

## Making Updates

After deployment, any changes are simple:

1. Edit content files in `content/`
2. Commit and push:
```bash
git add .
git commit -m "Update content"
git push
```
3. GitHub Actions will automatically rebuild and deploy
4. Changes appear on your site in 2-5 minutes

## Troubleshooting

### Site not showing up

- Check the "Actions" tab to see if deployment succeeded
- Verify Pages is enabled in Settings
- Check that the workflow shows a green checkmark

### Wrong URL structure

- Make sure `baseURL` in `hugo.toml` matches your site URL
- Rebuild: `hugo --minify`
- Commit and push

### Content not updating

- Check the Actions tab for build errors
- Verify you pushed to the `main` branch
- Wait a few minutes for the workflow to complete

## Custom Domain (Optional)

To use a custom domain like `terpsichore.info`:

1. Go to Settings → Pages
2. Under "Custom domain", enter your domain
3. Update your domain's DNS settings (see GitHub's documentation)
4. Update `baseURL` in `hugo.toml`:
   ```toml
   baseURL = "https://terpsichore.info/"
   ```

## Next Steps

Once deployed:
- Customize the theme further
- Add images and media
- Set up a contact form
- Monitor analytics
- Regular content updates

## Need Help?

- [Hugo Documentation](https://gohugo.io/documentation/)
- [GitHub Pages Help](https://docs.github.com/en/pages)
- [PaperMod Theme Guide](https://github.com/adityatelange/hugo-papermod/wiki)
