# BullGod Website - Astro Deployment Guide

## ✅ Project Status: Ready to Deploy

The website has been successfully converted to Astro and is ready for deployment to Vercel.

## 📁 Project Structure

```
bullgod-website/
├── public/              # Static assets (images, etc.)
│   ├── bullgodtransparent.png
│   ├── collection/      # Collection images
│   ├── tweets/          # Tweet screenshots
│   └── videos/          # Video thumbnails
├── src/
│   ├── pages/
│   │   └── index.astro  # Main page
│   └── styles/
│       └── global.css   # All styles (mobile responsive)
├── astro.config.mjs     # Astro configuration
├── package.json         # Dependencies
└── vercel.json          # Vercel config (optional)
```

## 🚀 Local Development

```bash
# Install dependencies (if not already done)
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📱 Mobile Responsive

The website is fully optimized for mobile devices with:
- Responsive typography using `clamp()`
- Flexible layouts that adapt to screen sizes
- Touch-friendly buttons and interactions
- Optimized images and spacing
- Media queries for 768px, 480px, and 360px breakpoints

## 🌐 Deploy to Vercel

### Option 1: Deploy via Vercel Dashboard

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Import your GitHub repository
4. Vercel will auto-detect Astro
5. Click "Deploy"

### Option 2: Deploy via CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

## ⚙️ Configuration

- **Framework**: Astro 4.15.0
- **Output**: Static
- **Adapter**: @astrojs/vercel/static
- **Node Version**: >=18.0.0

## ✨ Features

- ✅ Mobile responsive design
- ✅ All original content and styling preserved
- ✅ Tokenomics animation
- ✅ Collection carousel
- ✅ Copy-to-clipboard functionality
- ✅ Dropdown menus
- ✅ Smooth scrolling
- ✅ Optimized for performance

## 📝 Notes

- All assets are in the `public/` folder and are served at the root path
- CSS is imported in the Astro component frontmatter
- JavaScript is embedded in the page (can be extracted to separate file if needed)
- The build output goes to `.vercel/output/static/` when using the Vercel adapter

## 🔧 Troubleshooting

If you encounter issues:

1. **Build fails**: Run `npm install` to ensure all dependencies are installed
2. **Images not loading**: Verify assets are in the `public/` folder
3. **Styles not applying**: Check that CSS import is in the frontmatter

---

**Ready to deploy!** 🚀

