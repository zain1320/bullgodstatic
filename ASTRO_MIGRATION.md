# Astro Migration Guide

I've set up the basic Astro structure. To complete the migration:

## Next Steps

1. **Install dependencies:**
   ```bash
   cd bullgod-website
   npm install
   ```

2. **The HTML file needs to be converted to Astro format:**
   - Extract CSS from `<style>` tag to `src/styles/global.css`
   - Extract JavaScript from `<script>` tag to `public/script.js` or inline in components
   - Convert HTML to Astro component format in `src/pages/index.astro`

3. **Key changes needed:**
   - Replace `./` image paths with `/` (Astro public folder)
   - Convert inline styles to CSS classes where possible
   - Move JavaScript to `<script>` tags in Astro components (client-side)

## Current Structure

- ✅ `package.json` - Astro dependencies configured
- ✅ `astro.config.mjs` - Vercel adapter configured
- ✅ `src/` directory structure created
- ✅ `public/` folder with assets moved
- ⏳ Need to convert `index.html` to `src/pages/index.astro`

## Quick Conversion Tips

1. **Images:** Change `./bullgodtransparent.png` to `/bullgodtransparent.png`
2. **CSS:** Move `<style>` content to `src/styles/global.css` and import it
3. **JavaScript:** Keep in `<script>` tag in Astro component (runs client-side)
4. **Components:** Can be extracted later for better organization

The site will work the same way, just with Astro's build system!

