# Restaurant QR Menu System (2025 Edition)

A modern, mobile-first QR code menu system for restaurants built with 2025 web standards. Features smooth animations, skeleton loaders, and optimized for GitHub Pages deployment.

## Overview

The digital menu system consists of three main components:

1. **Main QR Page** (`index.html`) - QR code standee for customers to scan and view the menu
2. **Menu Viewer** (`viewer.html`) - Page with download/view options when QR is scanned
3. **Review Collection** (`review.html`) - QR code page for collecting Google Reviews

## Demo

Live demo: [https://desi-videsi.github.io/restaurent-files/](https://desi-videsi.github.io/restaurent-files/)

**Note:** Demo uses proprietary Desi Videsi Restaurant branding. Replace with your own when forking.

## 2025 Features

### Design & UX
- **Mobile-First Responsive** - Optimized for smartphones with progressive enhancement
- **Smooth Animations** - Fade-in, slide-up effects using modern CSS
- **Skeleton Loaders** - Visual feedback while images/QR codes load
- **Modern Typography** - System font stack for native look
- **Touch-Optimized** - 48px min touch targets, hover states
- **Print-Ready** - index.html optimized for 4x6" standee printing

### Technical
- **CSS Custom Properties** - Easy theming with CSS variables
- **CSS Grid Layouts** - Modern layout system
- **PDF.js Viewer Integration** - Web-based PDF viewing (no reader required)
- **Semantic HTML5** - Better accessibility
- **Optimized Loading** - Progressive image loading with fallbacks
- **Cross-Browser Compatible** - Works on all modern browsers

### Performance
- Minimal DOM manipulation
- Hardware-accelerated animations
- Efficient CSS (no redundant rules)
- Fast initial load
- Smooth 60fps transitions

## File Structure

```
├── index.html              # Main QR standee page
├── viewer.html             # Menu viewer with download/view options
├── review.html             # Google Review collection page
├── Menu Card.pdf           # Your restaurant menu (replace)
└── [Logo].png             # Your logo image (replace)
```

## Quick Start

### 1. Fork & Deploy
```bash
# Fork this repository
# Enable GitHub Pages in Settings → Pages → Source: main branch
```

### 2. Replace Content
**Must replace these proprietary files:**
- `Menu Card.pdf` - Your restaurant's menu
- `Desi Videsi Final edit Transparent Format.png` - Your logo

**Update in all 3 HTML files:**
- Restaurant name
- Address & Google Maps link
- Phone numbers
- Business hours
- Google Review link (review.html)
- Instagram handle (if applicable)

### 3. Customize Branding
Edit CSS variables in each file's `<style>` section:
```css
:root {
    --color-primary: #b8860b;        /* Your brand color */
    --color-primary-dark: #97710a;   /* Darker shade for hover */
    /* ... other variables ... */
}
```

## Customization Guide

### Colors
All colors use CSS custom properties - change once, updates everywhere:
- `--color-primary` - Main brand color
- `--color-primary-dark` - Hover/active states
- `--color-text` - Main text
- `--color-bg` - Background

### Spacing
Consistent spacing scale:
- `--spacing-xs` to `--spacing-2xl`
- Modify for tighter/looser layouts

### Animations
Adjust timing/easing:
```css
--transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
```

### Typography
Change font stack in `body` selector:
```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', ...;
```

## Print Usage

`index.html` includes print-optimized CSS for 4x6" standees:
1. Open index.html in browser
2. Print (Ctrl+P / Cmd+P)
3. Set paper size: 4" × 6"
4. Margins: Minimum

## Browser Support

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Technical Details

### Mobile-First Approach
Base styles target mobile, use `@media (min-width: ...)` for larger screens:
```css
/* Mobile base */
.element { font-size: 1rem; }

/* Desktop enhancement */
@media (min-width: 480px) {
    .element { font-size: 1.2rem; }
}
```

### Skeleton Loaders
Shimmer effect while content loads:
```css
@keyframes shimmer {
    0% { background-position: 200% 0; }
    100% { background-position: -200% 0; }
}
```

### QR Code Generation
Uses QRCode.js (CDN):
- High error correction level
- Responsive sizing (150px mobile, 180px desktop)
- Instant generation with skeleton placeholder

### PDF Viewing
**View Menu Online** button uses Mozilla's PDF.js:
```javascript
'https://mozilla.github.io/pdf.js/web/viewer.html?file=' + encodeURIComponent(pdfPath)
```
- Works without PDF reader installed
- Full web-based interface (zoom, search, page nav)
- Better mobile experience than raw PDF
- Stable external dependency (maintained by Mozilla)

**Download Menu** button:
```javascript
href = pdfPath  // Direct download
download = "Desi-Videsi-Menu.pdf"
```

## SEO Optimization

Each page includes:
- Descriptive `<title>` tags
- Meta descriptions
- Semantic HTML structure
- Accessible alt text

To improve further:
- Add Open Graph meta tags
- Add structured data (JSON-LD)
- Add sitemap.xml
- Submit to Google Search Console

## Accessibility Features

- Semantic HTML5 elements
- Descriptive alt text on images
- Sufficient color contrast
- Keyboard navigation support
- Touch-friendly tap targets (48px minimum)

## Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## Troubleshooting

**QR code not generating?**
- Check browser console for errors
- Verify QRCode.js CDN is accessible
- Ensure JavaScript is enabled

**PDF viewer not working?**
- Verify PDF file exists in GitHub repo
- Check PDF.js CDN: `mozilla.github.io/pdf.js`
- Try direct download button instead
- Ensure PDF file is accessible (not 404)

**Images not loading?**
- Verify file paths in GitHub repository
- Check filename encoding (spaces = %20)
- Confirm GitHub Pages is enabled

**Animations not smooth?**
- Check browser hardware acceleration
- Test on different devices
- Reduce animation complexity if needed

## Changelog

### v2.0 (2025)
- Complete rewrite with modern standards
- Mobile-first responsive design
- Added skeleton loaders
- CSS Grid layouts
- CSS custom properties
- Retained PDF.js viewer for better UX
- Improved animations
- Better accessibility
- Optimized performance

### v1.0 (2024)
- Initial release
- Basic QR menu system
- Desktop-first design

## License

**Code:** MIT License (see below)
**Content:** Logo, menu PDF, and Desi Videsi branding are proprietary - NOT included in license

```
MIT License

Copyright (c) 2025 Gopal Kedia

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Contact

Gopal Kedia
- Phone: +91 7894420103
- Restaurant: Desi Videsi (Demo only - use your own branding)

---

**Remember:** When forking, you MUST replace the logo, menu PDF, and all restaurant-specific information. These are not covered by the MIT license.
