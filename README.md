# CharadesCam Website

Official website for CharadesCam - The ultimate charades game with video recording.

## Overview

This is a static website built with plain HTML and Tailwind CSS. It's designed to be lightweight, fast, and easy to deploy.

## Structure

```
CharadesCamPage/
├── index.html          # Main landing page
├── privacy.html        # Privacy Policy (required for App Store)
├── terms.html          # Terms of Service (required for App Store)
├── support.html        # Support & FAQ page
├── assets/             # Images and media files from the app
│   ├── logo-icon.png
│   ├── logo.png
│   ├── favicon.png
│   ├── how_to_play_*.png
│   └── deck/           # Theme deck images
└── README.md           # This file
```

## Features

- **Responsive Design**: Works on all devices from mobile to desktop
- **No Build Process**: Pure HTML/CSS, no compilation needed
- **CDN-Based**: Uses Tailwind CSS via CDN
- **Fast Loading**: Optimized for performance
- **App Store Ready**: Includes all required legal pages

## Local Development

Simply open `index.html` in your web browser. No server or build process required!

For a better development experience with live reloading, you can use:

```bash
# Using Python (comes pre-installed on macOS)
python3 -m http.server 8000

# Using Node.js
npx serve

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Deployment Options

### Option 1: GitHub Pages (Recommended - Free & Easy)

1. Create a new GitHub repository
2. Push this directory to the repository:
   ```bash
   cd CharadesCamPage
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
   git push -u origin main
   ```
3. Go to your repository Settings > Pages
4. Select "Deploy from a branch" and choose "main" branch
5. Your site will be live at `https://YOUR_USERNAME.github.io/YOUR_REPO/`

**Custom Domain:**
- In repository settings, add your custom domain
- Update your DNS settings with a CNAME record pointing to `YOUR_USERNAME.github.io`

### Option 2: Netlify (Free with drag-and-drop)

1. Go to [netlify.com](https://www.netlify.com/)
2. Sign up for a free account
3. Drag and drop the `CharadesCamPage` folder onto the Netlify dashboard
4. Your site is live instantly!
5. Optional: Configure a custom domain in site settings

**Deploy via Git (Alternative):**
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
cd CharadesCamPage
netlify deploy --prod
```

### Option 3: Vercel (Free with excellent performance)

1. Go to [vercel.com](https://vercel.com/)
2. Sign up and import your GitHub repository
3. Vercel will auto-detect it's a static site
4. Deploy!

**Using Vercel CLI:**
```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
cd CharadesCamPage
vercel --prod
```

### Option 4: Cloudflare Pages (Free with CDN)

1. Go to [Cloudflare Pages](https://pages.cloudflare.com/)
2. Connect your GitHub account
3. Select your repository
4. Configure:
   - Build command: (leave empty)
   - Build output directory: `/`
5. Deploy!

### Option 5: Traditional Web Hosting

Upload the entire `CharadesCamPage` directory to your web hosting via FTP/SFTP.

## Customization

### Update App Store Links

When your app is approved, update the download links in:
- `index.html` (2 locations: hero section and CTA section)

Replace `#` with your actual App Store and Google Play URLs:

```html
<!-- iOS App Store -->
<a href="https://apps.apple.com/app/YOUR_APP_ID">

<!-- Google Play Store -->
<a href="https://play.google.com/store/apps/details?id=tech.hoshiko.charadescam">
```

### Update Contact Emails

Replace placeholder emails if needed:
- `support@charades.cam`
- `privacy@charades.cam`
- `legal@charades.cam`
- `bugs@charades.cam`
- `feedback@charades.cam`
- `info@charades.cam`

Set up email forwarding or create real inboxes for these addresses.

### Add Analytics (Optional)

To track visitor statistics, add Google Analytics or similar:

1. Create a Google Analytics account
2. Get your tracking ID
3. Add this before `</head>` in all HTML files:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Update Copyright Year

The footer shows "© 2025 CharadesCam by Hoshiko Tech". Update this as needed.

## For App Store Submission

Apple and Google require certain pages for app submission:

✅ **Privacy Policy** - `privacy.html`
- Explains data collection (none in this case)
- Required for both App Store and Google Play

✅ **Terms of Service** - `terms.html`
- User agreement and legal terms
- Required for both stores

✅ **Support URL** - `support.html`
- Help and contact information
- Required field in app submission forms

When submitting your app, use these URLs:
- **Privacy Policy URL**: `https://yourdomain.com/privacy.html`
- **Terms of Service URL**: `https://yourdomain.com/terms.html`
- **Support URL**: `https://yourdomain.com/support.html`

## SEO Optimization

The site is already SEO-friendly with:
- Semantic HTML
- Meta descriptions
- Proper heading hierarchy
- Alt text for images
- Mobile responsive design

To improve further:
1. Submit your sitemap to Google Search Console
2. Add Open Graph tags for social media sharing
3. Optimize images (already done via assets)

## Performance

The site is already optimized:
- ✅ No JavaScript frameworks (pure HTML/CSS)
- ✅ Tailwind CSS via CDN (cached globally)
- ✅ Optimized images
- ✅ Minimal file size
- ✅ Fast loading (< 1s)

**Lighthouse Score Target:** 90+ across all metrics

## Browser Support

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Maintenance

### Regular Updates

- Keep legal pages current (review annually)
- Update screenshots when app UI changes
- Add new themes as they're added to the app
- Update download links when app is published

### Monitoring

Consider setting up:
- Uptime monitoring (e.g., UptimeRobot)
- Analytics for visitor tracking
- Contact form submissions (if you add one)

## Assets

All assets are copied from the CharadesCam mobile app:
- Logo and icons
- How-to-play screenshots
- Theme deck images

To update assets:
```bash
cp -r ../CharadesCam/assets ./assets
```

## License

© 2025 CharadesCam by Hoshiko Tech. All rights reserved.

## Support

For questions about the website, contact:
- Email: info@charades.cam
- For app support: support@charades.cam

---

**Ready to deploy!** Choose your deployment method above and get your site live in minutes.
