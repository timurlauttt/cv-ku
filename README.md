# Atlas Astro

A modern, performant blog template built with Astro and Tailwind CSS.

## Features

✨ **Performance-First**: Zero JavaScript by default, blazing fast page loads
🎨 **Tailwind CSS**: Utility-first styling with custom Atlas theme
📝 **Content Collections**: Type-safe blog posts with MDX support
🌙 **Dark Mode**: Built-in dark mode with localStorage persistence
🔍 **SEO Optimized**: Meta tags, sitemap, and RSS feed included
⚡ **View Transitions**: Smooth page transitions with Astro's View Transitions API
📱 **Responsive**: Mobile-first design that works on all devices

## Tech Stack

- **Astro 5.x** - Static site generator
- **Tailwind CSS 3.x** - Styling
- **TypeScript** - Type safety
- **MDX** - Enhanced markdown for blog posts
- **@astrojs/sitemap** - Automatic sitemap generation
- **@astrojs/rss** - RSS feed for blog

## Getting Started

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

Visit http://localhost:4321 to see your site.

### Build

```bash
npm run build
```

The built site will be in the `dist/` folder, ready to deploy.

### Preview Production Build

```bash
npm run preview
```

## Project Structure

```
/
├── public/           # Static assets (images, fonts, etc.)
├── src/
│   ├── components/   # Reusable Astro components
│   │   ├── Header.astro
│   │   └── Footer.astro
│   ├── content/      # Content collections
│   │   ├── config.ts
│   │   └── blog/     # Blog posts in Markdown/MDX
│   ├── layouts/      # Page layouts
│   │   └── Layout.astro
│   ├── pages/        # File-based routing
│   │   ├── index.astro
│   │   ├── blog.astro
│   │   ├── blog/
│   │   │   └── [slug].astro
│   │   ├── contact.astro
│   │   ├── uses.astro
│   │   └── rss.xml.js
│   └── styles/       # Global styles
│       └── global.css
├── astro.config.mjs  # Astro configuration
├── tailwind.config.mjs # Tailwind configuration
└── package.json
```

## Customization

### Site Configuration

Edit `astro.config.mjs` to update the site URL:

```js
export default defineConfig({
  site: 'https://your-domain.com',
  // ...
});
```

### Theme Colors

Customize colors in `tailwind.config.mjs`:

```js
colors: {
  primary: "#072344",
  secondary: "#00aaa1",
  // ... more colors
}
```

### Adding Blog Posts

Create new blog posts in `src/content/blog/`:

```markdown
---
title: 'Your Post Title'
description: 'Post description'
pubDate: 2026-02-06
tags: ['tag1', 'tag2']
---

Your content here...
```

## Performance

This site is optimized for maximum performance:

- **Lighthouse Score**: 100/100 (Performance, Accessibility, Best Practices, SEO)
- **First Contentful Paint**: < 0.5s
- **Time to Interactive**: < 1s
- **Bundle Size**: Minimal (only essential CSS and JS)

## Deployment

Deploy to any static hosting service:

- **Netlify**: `netlify deploy --prod --dir=dist`
- **Vercel**: `vercel --prod`
- **Cloudflare Pages**: Connect your Git repository
- **GitHub Pages**: Use GitHub Actions

## License

MIT License - feel free to use this template for your own projects.

## Credits

Original design: Red Pixel Themes
Migrated to Astro: Optimized for performance and modern web standards
