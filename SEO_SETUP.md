# SEO Setup Instructions

## Open Graph Image Setup

To complete the SEO setup, you need to create an Open Graph image for social media sharing:

### 1. Create og-image.png
- **Location:** `public/og-image.png`
- **Dimensions:** 1200x630 pixels (1.91:1 aspect ratio)
- **Format:** PNG (recommended) or JPG
- **Content:** A screenshot or custom image of your portfolio

### 2. Recommended Content for og-image.png:
- Your name prominently displayed
- "Data Analyst & BI Developer" subtitle
- Key technologies: Power BI, Python, SQL
- Your portfolio branding/colors
- Clean, professional design

### 3. Tools to Create og-image.png:
- **Canva:** Design from scratch
- **Screenshot:** Take a high-quality screenshot of your hero section
- **Figma/Photoshop:** Custom design
- **Online Generators:** Use tools like "Open Graph Image Generator"

### 4. Update Domain URLs
Replace the placeholder URLs in `app/layout.tsx`:
- `metadataBase`: Set to your actual domain (e.g., `https://yourportfolio.com`)
- `canonical`: Set to your actual domain
- `jsonLd.url`: Set to your actual domain

### 5. Test Your SEO
Use these tools to verify your SEO setup:
- **Google Rich Results Test:** https://search.google.com/test/rich-results
- **Open Graph Preview:** https://www.opengraph.xyz/
- **Twitter Card Validator:** https://cards-dev.twitter.com/validator

## Current SEO Features Implemented:
✅ Title tag optimization
✅ Meta description
✅ Open Graph tags (og:title, og:description, og:image, og:url)
✅ Twitter Card tags
✅ Keywords meta tag
✅ Structured data (JSON-LD)
✅ Canonical URL
✅ Robots meta tag
✅ Font preloading
✅ Accessibility features