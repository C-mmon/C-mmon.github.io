# Chirpy Jekyll Theme Setup Instructions

## Prerequisites Installation

### 1. Install Ruby (Required)
- Download Ruby installer from: https://rubyinstaller.org/downloads/
- Choose "Ruby+Devkit 3.x.x (x64)" - latest stable version
- Run installer and follow the setup wizard
- Make sure to check "Add Ruby executables to your PATH"

### 2. Install Jekyll and Bundler
After Ruby is installed, open PowerShell and run:
```powershell
gem install jekyll bundler
```

### 3. Install Project Dependencies
Navigate to your project folder and install dependencies:
```powershell
cd "c:\Users\Aniket\OneDrive\Desktop\CmmonPersonalWebsite\C-mmon.github.io"
bundle install
```

### 4. Build and Serve the Site
```powershell
bundle exec jekyll serve
```

Your site will be available at: http://localhost:4000

## Customization

### 1. Edit _config.yml
Update the following fields in `_config.yml`:

```yaml
title: Your Name # Change this to your name
tagline: Developer & Tech Writer # Your tagline
description: Your personal blog description
url: "https://yourusername.github.io" # Your GitHub Pages URL

github:
  username: yourusername # Your GitHub username

social:
  name: Your Full Name
  email: your.email@example.com
  links:
    - https://github.com/yourusername
    - https://linkedin.com/in/yourprofile
```

### 2. Create Your First Post
- Posts go in the `_posts` folder
- Name format: `YYYY-MM-DD-title.md`
- Example: `2025-05-26-my-first-post.md`

### 3. Customize About Page
- Edit `_tabs/about.md` to update your about page

### 4. Add Your Photo
- Add your photo to `assets/img/`
- Update avatar in `_config.yml`

## Features You Get

✅ **Modern Blog Theme**
- Dark/Light mode toggle
- Responsive design
- SEO optimized
- Fast loading

✅ **Rich Content Support**
- Markdown posts
- Syntax highlighting
- Math equations (LaTeX)
- Mermaid diagrams
- Image galleries

✅ **Professional Features**
- Table of contents
- Related posts
- Comment system support
- Search functionality
- Archive pages
- Tag/Category organization

✅ **Analytics & SEO**
- Google Analytics support
- SEO meta tags
- Sitemap generation
- RSS feeds

## Commands Reference

```powershell
# Serve locally (development)
bundle exec jekyll serve

# Build for production
bundle exec jekyll build

# Update theme
bundle update jekyll-theme-chirpy
```

## GitHub Pages Deployment

1. Push your changes to GitHub
2. Go to Settings > Pages in your repository
3. Set source to "GitHub Actions"
4. The site will automatically build and deploy

## Troubleshooting

If you encounter issues:

1. **Ruby not found**: Make sure Ruby is in your PATH
2. **Bundle command not found**: Run `gem install bundler`
3. **Permission errors**: Run PowerShell as Administrator
4. **Build errors**: Check `_config.yml` syntax

## Resources

- [Chirpy Documentation](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)
