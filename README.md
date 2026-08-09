# Davince Visuals Website

Official static website for **Davince Visuals** featuring photography, film production, digital art, and creative IT services in Uganda.

🌐 Live site: https://davincevisuals.com/

## Features

- SEO-focused homepage metadata and Open Graph tags
- Structured data (`LocalBusiness`, `Service`, `ImageGallery`)
- Responsive single-page layout with service, portfolio, booking, and contact sections
- Accessible navigation, skip-link, and descriptive image alt text
- Booking/contact forms with real-time validation feedback
- Externalized CSS for caching and easier maintenance

## Project Structure

- `index.html` — main website page
- `thankyou.html` — post-submission confirmation page
- `styles.css` — shared stylesheet
- `*.jpg|*.png` — brand and portfolio assets

## Local Development

This is a static site and does not require a build step.

### Option 1: Open directly
Open `index.html` in a browser.

### Option 2: Run a local static server (recommended)
```bash
cd davince-visuals
python -m http.server 8080
```
Then visit http://localhost:8080.

## Deployment

The site is configured for GitHub Pages with the custom domain in `CNAME`.

- Primary URL: https://davincevisuals.com/
- Thank-you page: https://davincevisuals.com/thankyou.html

## Performance & Image Optimization Notes

Some source images are currently large and should be optimized before production refreshes:

- `20260602_190647(1).jpg` (~9.7 MB)
- `background.jpg` (~3.4 MB)
- `portfolio2.jpg` (~2.7 MB)
- `portfolio3.jpg` (~3.3 MB)

Recommended approach:

1. Convert large images to **WebP** (and keep JPEG fallback if needed).
2. Resize to display-appropriate dimensions before upload.
3. Use responsive images (`srcset`/`sizes`) for gallery and hero assets.
4. Target <500 KB for full-width hero images where quality allows.

## SEO & Accessibility Checklist

- Canonical URL and favicon/apple-touch-icon set
- Theme color and compatibility meta tags included
- Descriptive alt text on gallery and brand images
- Structured data embedded for business and services

## Contact

- Email: info@davincevisuals.com
- Phone: +256 774 231 123
