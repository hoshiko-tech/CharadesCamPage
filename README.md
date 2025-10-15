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


## Customization

### Update App Store Links

When your app is approved, update the download links in:
- `index.html` (2 locations: hero section and CTA section)

Replace `#` with your actual App Store and Google Play URLs:

```html
<!-- iOS App Store -->
<a href="https://apps.apple.com/app/APP_ID">

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
- **Privacy Policy URL**: `https://charades.cam/privacy.html`
- **Terms of Service URL**: `https://charades.cam/terms.html`
- **Support URL**: `https://charades.cam/support.html`

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

© 2025 CharadesCam by Hoshiko Tech Ltd. All rights reserved.

## Support

For questions about the website, contact:
- Email: info@charades.cam
- For app support: support@charades.cam

---
