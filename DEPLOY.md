# 🚀 Quick Deployment Guide

## Step 1: Upload to GitHub

1. **Create a new GitHub repository:**
   - Go to https://github.com/new
   - Name it `bullgod-website` (or any name you prefer)
   - Make it **Public** or **Private** (your choice)
   - **Don't** initialize with README, .gitignore, or license (we already have these)

2. **Push this folder to GitHub:**
   ```bash
   cd bullgod-website
   git init
   git add .
   git commit -m "Initial commit - BullGod website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/bullgod-website.git
   git push -u origin main
   ```
   Replace `YOUR_USERNAME` with your GitHub username.

## Step 2: Deploy to Vercel

1. **Go to Vercel:**
   - Visit https://vercel.com
   - Sign in with GitHub

2. **Import your repository:**
   - Click "Add New Project"
   - Select your `bullgod-website` repository
   - Vercel will auto-detect it as a static site
   - Click "Deploy"

3. **That's it!** Your site will be live in seconds.

## Alternative: Deploy via Vercel CLI

If you prefer command line:

```bash
cd bullgod-website
npm i -g vercel
vercel
```

Follow the prompts. Your site will be deployed!

## 📝 Notes

- The `vercel.json` file is already configured for static hosting
- All paths in `index.html` use relative paths (./), so everything will work correctly
- The videos folder is empty - you can add video thumbnails later if needed
- Your site will get a URL like: `https://bullgod-website.vercel.app`

## ✅ Verification

After deployment, check:
- ✅ Logo displays correctly
- ✅ Collection images load
- ✅ Tweet images display
- ✅ All links work
- ✅ Mobile responsive design works

