---
title: "Blog Guide"
date: 2024-11-21
categories: [Blog]
tags: [blog]
layout: post
---

# How to Use This Blog Template

This guide will help you set up your blog using GitHub's web interface.

## 1. Create Your Repository

1. Go to [chirpy-starter template](https://github.com/cotes2020/chirpy-starter)
2. Click the green "Use this template" button
3. Choose "Create a new repository"
4. Name your repository: `<YOUR_USERNAME>.github.io`
5. Select "Public" repository
6. Click "Create repository from template"

## 2. Configure Your Blog

1. Go to your new repository
2. Edit `_config.yml` (click the pencil icon):
   ```yml
   title: Your Blog Title
   tagline: Your blog tagline
   description: Your blog description
   url: 'https://<YOUR_USERNAME>.github.io'
   
   github:
     username: <YOUR_USERNAME>
   
   social:
     name: Your Name
     email: your.email@example.com
     links:
       - https://github.com/<YOUR_USERNAME>

   # URL for the avatar on sidebar
   avatar:

   ```
3. Commit changes

## 3. Create Your First Post

1. Navigate to `_posts` folder
2. Click "Add file" → "Create new file"
3. Name your file: `YYYY-MM-DD-title.md` (e.g., `2024-03-21-first-post.md`)
4. Add post content:
   ```markdown
   ---
   title: "Your Post Title"
   date: YYYY-MM-DD
   categories: [Category1, Category2]
   tags: [tag1, tag2]
   ---

   Your content here...
   ```
5. Commit changes

## 4. Enable GitHub Pages

1. Go to repository Settings
2. Click "Pages" in the left sidebar
3. Under "Source":
   - Select "GitHub Actions" as the source
4. Wait a few minutes for your site to deploy

## 5. Writing Tips

### Adding Images
1. Upload images to `assets/img/`
2. Reference in posts:
   ```markdown
   ![Alt text](/assets/img/your-image.jpg)
   ```

### Categories and Tags
- Add in front matter:
  ```markdown
  ---
  categories: [Programming, Python]
  tags: [code, tutorial]
  ---
  ```

## 6. Customization

### Add Custom Pages
1. Create new `.md` file in _tabs folder
2. Add front matter:
   ```markdown
   ---
   layout: categories
   icon: fas fa-stream
   order: 5
   ---
   ```
## 7. Updating

Your site will automatically use the latest theme version when GitHub Actions runs.

---

For more detailed documentation, visit [Chirpy theme docs](https://chirpy.cotes.page/).