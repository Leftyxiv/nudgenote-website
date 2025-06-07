# NudgeNote Website

Marketing website for NudgeNote - the iOS app that helps you maintain meaningful connections.

## Tech Stack

- **Framework**: Astro (Static Site Generator)
- **Styling**: Vanilla CSS with CSS Custom Properties
- **Hosting**: Deploy to any static host (Netlify, Vercel, etc.)

## Getting Started

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
nudgenote-website/
├── public/
│   ├── .well-known/
│   │   └── apple-app-site-association  # iOS deep linking
│   ├── favicon.svg
│   └── robots.txt
├── src/
│   ├── components/
│   │   ├── Header.astro               # Site navigation
│   │   ├── Footer.astro               # Site footer
│   │   └── Analytics.astro            # Analytics setup (disabled by default)
│   ├── layouts/
│   │   └── Layout.astro               # Base layout with SEO
│   └── pages/
│       ├── index.astro                # Landing page
│       ├── privacy.astro              # Privacy policy
│       ├── terms.astro                # Terms of service
│       ├── support.astro              # Support page
│       └── sitemap.xml.ts             # Dynamic sitemap
└── astro.config.mjs                   # Astro configuration
```

## Key Features

- ✅ Mobile-responsive design
- ✅ Performance optimized (<1MB, <3s load time)
- ✅ SEO optimized with meta tags
- ✅ WCAG 2.1 Level AA accessible
- ✅ Privacy-focused (no tracking by default)
- ✅ Apple App Site Association for iOS deep linking

## Configuration

### Analytics

Analytics are disabled by default. To enable:

1. Choose a privacy-focused provider (Plausible, Fathom, or Simple Analytics)
2. Edit `src/components/Analytics.astro` with your credentials
3. Import Analytics in `src/layouts/Layout.astro`

### Apple App Site Association

Update `/public/.well-known/apple-app-site-association` with your:
- Team ID
- App Bundle ID

### App Store Links

Replace `https://apps.apple.com/app/id1234567890` with your actual App Store URL throughout the site.

## Deployment

The site is static and can be deployed to any static hosting provider:

```bash
# Build the site
npm run build

# Deploy the 'dist' folder to your host
```

### Recommended Hosts

- Netlify (automatic deploys from Git)
- Vercel (automatic deploys from Git)
- Cloudflare Pages
- GitHub Pages

## Performance

The site is optimized for performance:
- Minimal JavaScript (Astro ships zero JS by default)
- Inlined critical CSS
- System fonts
- Optimized images (when added)
- HTML compression

## Brand Guidelines

- **Primary Color**: #14B8A6 (Teal)
- **Secondary Color**: #8B5CF6 (Purple)
- **Gradient**: 135deg from teal to purple
- **Typography**: System font stack
- **Border Radius**: Rounded corners for friendly feel
- **Shadows**: Soft shadows for depth

## License

Copyright © 2025 NudgeNote. All rights reserved.