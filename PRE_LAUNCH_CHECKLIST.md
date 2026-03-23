# Pre-Launch Checklist for Portfolio

## ✅ TEXT CONTENT FIXES COMPLETED
- [x] "From Data To Insights" → "From Data to Insights" (lowercase 'to')
- [x] "Convent school" → "Convent School" (title case)
- [x] "Fiit-Jee" → "FIITJEE" (official spelling)
- [x] "Power BI" vs "PowerBi" → "Power BI" used consistently
- [x] "GitHub" vs "Github" → "GitHub" used consistently
- [x] "LinkedIn" vs "Linkedin" → "LinkedIn" used consistently
- [x] Punctuation consistency checked
- [x] Double spaces removed

## 🔍 PERFORMANCE CHECKLIST
- [ ] Lighthouse score > 90 on all metrics (Performance, Accessibility, Best Practices, SEO)
- [ ] Mobile responsiveness tested (iPhone, Android, tablet)
- [ ] Cross-browser tested (Chrome, Firefox, Safari, Edge)
- [ ] Page load time < 3 seconds on 3G
- [ ] Core Web Vitals: LCP < 2.5s, FID < 100ms, CLS < 0.1
- [ ] Images optimized (WebP format, lazy loading)
- [ ] Bundle size < 500KB (check with `npm run build`)

## ⚙️ FUNCTIONALITY CHECKLIST
- [ ] All navigation links work (smooth scroll to sections)
- [ ] Contact form submits successfully (EmailJS integration)
- [ ] Resume download works (KOUSHIK__CV.docx)
- [ ] External links open in new tab with rel="noopener noreferrer"
- [ ] Dark/light mode toggle persists across sessions
- [ ] Particle animations respect `prefers-reduced-motion`
- [ ] Form validation works (name, email, message required)
- [ ] reCAPTCHA verification functional
- [ ] Modal dialogs accessible (ESC to close, focus management)
- [ ] Skip link works for keyboard navigation

## 📝 CONTENT CHECKLIST
- [ ] All dates verified and correct (education, experience, projects)
- [ ] All project descriptions accurate and professional
- [ ] No placeholder text remaining ("Lorem ipsum", etc.)
- [ ] Contact information current (+91 6305544031, lingalakoushik@gmail.com)
- [ ] Social media links working (LinkedIn, GitHub)
- [ ] Resume file up-to-date and professional
- [ ] Alt text added to all images and visual mockups
- [ ] Spelling and grammar checked throughout

## 📊 ANALYTICS & TRACKING
- [ ] Google Analytics or Plausible added (update .env.local)
- [ ] Track resume downloads (event: 'resume_download')
- [ ] Track contact form submissions (event: 'contact_form_submit')
- [ ] Track project modal opens (event: 'project_view', project_name)
- [ ] Track social media clicks (event: 'social_click', platform)
- [ ] Track navigation clicks (event: 'nav_click', section)

## 🔍 SEO & METADATA
- [ ] Open Graph image created (og-image.png, 1200x630px)
- [ ] Domain URLs updated in layout.tsx (replace lingalakoushik.dev)
- [ ] Meta title and description optimized
- [ ] Structured data (JSON-LD) validated with Google's tool
- [ ] Sitemap.xml generated (optional)
- [ ] Robots.txt configured (optional)

## 🚀 DEPLOYMENT CHECKLIST
- [ ] Environment variables configured (.env.local)
- [ ] Build successful (`npm run build`)
- [ ] Preview deployment tested (Vercel/Netlify preview)
- [ ] Domain configured (custom domain if not using platform default)
- [ ] SSL certificate valid (HTTPS)
- [ ] 404 page customized
- [ ] Favicon and app icons configured

## 🧪 TESTING CHECKLIST
- [ ] Accessibility: WAVE tool, axe DevTools, screen reader testing
- [ ] Performance: PageSpeed Insights, WebPageTest
- [ ] SEO: Google Search Console, Rich Results Test
- [ ] Mobile: Chrome DevTools device emulation
- [ ] Forms: Submission testing, validation, error handling
- [ ] Links: All internal/external links functional
- [ ] Images: All images load, proper alt text
- [ ] Console: No JavaScript errors in production

## 📋 FINAL VERIFICATION
- [ ] Portfolio loads in incognito mode (no cached issues)
- [ ] All animations smooth and not janky
- [ ] Text readable on all backgrounds
- [ ] Color contrast meets WCAG AA standards
- [ ] Touch targets minimum 44px on mobile
- [ ] No horizontal scroll on any device
- [ ] Print styles work (for resume printing)

---

## Quick Commands for Testing

```bash
# Performance testing
npm run build && npx serve@latest out -p 3000

# Lighthouse testing
npx lighthouse http://localhost:3000 --output html --output-path ./lighthouse-report.html

# Bundle analysis
npx @next/bundle-analyzer
```

## Environment Variables Template (.env.local)

```env
# EmailJS Configuration
NEXT_PUBLIC_EMAILJS_SERVICE_ID=your_service_id
NEXT_PUBLIC_EMAILJS_TEMPLATE_ID=your_template_id
NEXT_PUBLIC_EMAILJS_PUBLIC_KEY=your_public_key
NEXT_PUBLIC_RECAPTCHA_SITE_KEY=your_recaptcha_site_key

# Analytics (choose one)
NEXT_PUBLIC_GA_ID=G-XXXXXXXXXX
NEXT_PUBLIC_PLAUSIBLE_DOMAIN=yourdomain.com

# Domain for canonical URLs
NEXT_PUBLIC_DOMAIN=https://yourportfolio.com
```

Remember to test everything thoroughly before going live! 🎉