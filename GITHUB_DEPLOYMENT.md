# 🚀 GitHub Pages Deployment Guide

## ✅ Setup Complete!
Your Chirpy Jekyll theme is now ready for GitHub Pages deployment with GitHub Actions.

## 📋 Step-by-Step GitHub Deployment

### 1. **Customize Your Site Configuration**

Edit `_config.yml` with your information:

```yaml
# Basic Site Info
title: Your Name                    # Your name or site title
tagline: Developer & Tech Writer    # Your subtitle/tagline
description: >-                     # Brief description for SEO
  Your personal blog about web development, programming, and technology.

# GitHub Pages URL (IMPORTANT!)
url: "https://yourusername.github.io"  # Replace with YOUR GitHub username

# Your Social Links
github:
  username: yourusername            # Your GitHub username

social:
  name: Your Full Name
  email: your.email@example.com
  links:
    - https://github.com/yourusername
    - https://linkedin.com/in/yourprofile

# Timezone (optional)
timezone: America/New_York          # Change to your timezone
```

### 2. **Push to GitHub**

```powershell
# Stage all files
git add .

# Commit your changes
git commit -m "Setup Chirpy Jekyll theme for GitHub Pages"

# Push to GitHub
git push origin main
```

### 3. **Enable GitHub Pages**

1. Go to your repository on GitHub.com
2. Click **Settings** tab
3. Scroll down to **Pages** section (left sidebar)
4. Under **Source**, select **GitHub Actions**
5. Save the changes

### 4. **That's It!** 🎉

GitHub will automatically:
- Build your Jekyll site
- Deploy it to `https://yourusername.github.io`
- Update it every time you push changes

## 📝 Creating Your First Blog Post

Create a new file in `_posts/` folder:

**File name format:** `YYYY-MM-DD-title.md`
**Example:** `2025-05-26-my-first-post.md`

```markdown
---
title: My First Blog Post
date: 2025-05-26 12:00:00 +0000
categories: [Programming, Web Development]
tags: [javascript, tutorial]
---

# My First Post

This is my first blog post using Jekyll and GitHub Pages!

## Features I Love

- Automatic deployment
- Beautiful theme
- Markdown support
- SEO optimization

```

## 🎨 Customization Tips

### Update About Page
Edit `_tabs/about.md`:

```markdown
---
# the default layout is 'page'
icon: fas fa-info-circle
order: 4
---

# About Me

I'm a passionate developer who loves creating amazing web applications...

## Skills
- JavaScript/TypeScript
- React/Next.js
- Node.js
- Python
```

### Add Your Photo
1. Add your photo to `assets/img/avatar.jpg`
2. Update `_config.yml`:
```yaml
avatar: "/assets/img/avatar.jpg"
```

## 📊 Analytics & SEO (Optional)

Add Google Analytics to `_config.yml`:
```yaml
analytics:
  google:
    id: G-XXXXXXXXXX  # Your Google Analytics ID
```

## 🔧 Local Development (Optional)

If you want to test locally before pushing:

1. **Install Ruby** (Windows): https://rubyinstaller.org/
2. **Install dependencies:**
```powershell
gem install jekyll bundler
bundle install
```
3. **Run locally:**
```powershell
bundle exec jekyll serve
```
4. **Visit:** http://localhost:4000

## 📦 What You Get

✅ **Professional Blog Platform**
- Modern, responsive design
- Dark/light mode toggle
- Mobile-friendly
- Fast loading

✅ **Rich Content Features**
- Markdown posts
- Syntax highlighting
- Math equations (LaTeX)
- Mermaid diagrams
- Table of contents

✅ **SEO & Analytics**
- Search engine optimization
- Google Analytics support
- Automatic sitemap
- RSS feeds

✅ **GitHub Integration**
- Automatic deployment
- Version control
- Free hosting
- Custom domain support

## 🔗 Useful Links

- **Your Site:** `https://yourusername.github.io` (after setup)
- **Repository:** Your GitHub repository
- **Chirpy Docs:** https://github.com/cotes2020/jekyll-theme-chirpy/wiki
- **Jekyll Docs:** https://jekyllrb.com/docs/

## 🆘 Troubleshooting

**Build Failed?**
- Check `_config.yml` syntax
- Make sure you updated the `url` field
- Check GitHub Actions tab for error details

**Site Not Loading?**
- Verify GitHub Pages is enabled
- Check if the repository name is correct
- Wait 5-10 minutes for first deployment

**Need Local Development?**
- Follow Ruby installation steps above
- Make sure to run `bundle install` first
