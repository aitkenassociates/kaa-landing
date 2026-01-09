# KAA Landing Page - Project Backlog

**Project:** Karen Aitken & Associates - Landscape Architecture Landing Page
**Last Updated:** 2026-01-09
**Tech Stack:** Astro 5.7.5+, Tailwind CSS 4, TypeScript, SCSS

---

## Reference Documents

### Notion & Plan MB Files

> **Note:** No Notion exports or Plan MB files were found in this repository at the time of backlog creation. If these documents exist externally, they should be:
> 1. Added to a `/docs/planning/` directory in this repository
> 2. Referenced with links if stored in external systems (Notion, Google Drive, etc.)

**TODO:** Add links to external planning documents here:
- [ ] Notion workspace link: _[Add link]_
- [ ] Plan MB documents: _[Add links]_
- [ ] Design mockups: _[Add links]_
- [ ] Brand guidelines: _[Add links]_

---

## Current State Summary

### Completed Features

#### Homepage (`src/pages/index.astro`)
- [x] Hero section with full-screen background image
- [x] Company branding: "Karen Aitken & Associates"
- [x] Tagline: "Creating California gardens for the decades"
- [x] CTA buttons: "Learn More" and "Get Started"
- [x] ContentMedia section with company description
- [x] Tabs component (Design Ideation, Conceptual Visualization, Nature Realization)
- [x] Stats/Counter section (900+ Projects, 25K+ Landscapes, 4M+ Plans, 5K+ Persons)
- [x] Starting Plans/Pricing section (3 tiers: $1,000, $2,000, $3,000)
- [x] Testimonial section with Jack Smith quote
- [x] FAQ section with 7 landscape design questions
- [x] Call-to-Action section linking to Typeform

#### Header/Navigation (`src/components/Header.astro`, `Navigation.astro`)
- [x] Logo component
- [x] Main navigation with dropdown support
- [x] Mobile responsive toggle
- [x] Skip links for accessibility
- [x] Current menu items: Home, About, Portfolio, Projects (dropdown), Contact Us

#### Footer (`src/components/Footer.astro`)
- [x] Navigation links section
- [x] Projects links section
- [x] Social media links (Houzz, Instagram, Facebook, YouTube)
- [x] Logo and tagline
- [x] Copyright notice
- [x] Developer credit

#### Components
- [x] Hero.astro - Full-screen hero with background image
- [x] Counter.astro - Animated statistics display
- [x] ContentMedia.astro - Image + text layout component
- [x] Feature.astro - Feature highlight component
- [x] CallToAction.astro - CTA section with Typeform link
- [x] ExternalLink.astro - External link with icon
- [x] ExternalLinkSocial.astro - Social media link component

---

## Backlog Items

### High Priority

#### Content Pages
- [x] **About Page** - ~~Currently links to `/blog/` (placeholder)~~ COMPLETED
  - ~~Create dedicated About page with company history~~
  - ~~Team member profiles~~
  - ~~Company philosophy/mission~~

- [ ] **Portfolio Page** - Exists but needs KAA-specific content
  - Replace sample projects with actual KAA portfolio items
  - Add project categories/filtering

- [ ] **Contact Page** - Dedicated contact page needed
  - Contact form integration
  - Office location/map
  - Business hours
  - Phone/email info

#### Project Category Pages
- [ ] **Residential Projects** - Currently links to `/accessibility-statement` (placeholder)
- [ ] **Commercial Projects** - Currently links to `/accessible-components` (placeholder)
- [ ] **Civic Projects** - Currently links to `/color-contrast-checker` (placeholder)

### Medium Priority

#### Content & Media
- [ ] Replace placeholder images with actual KAA project photos
  - Hero background image
  - Tab panel images (currently all use `garden-2-small.jpg`)
  - Pricing card images
- [ ] Add real testimonials from clients
- [ ] Update FAQ content based on actual client questions
- [ ] Add more project case studies to portfolio

#### Navigation & Structure
- [x] ~~Fix About link (currently points to `/blog/`)~~ COMPLETED
- [ ] Create proper project category pages
- [ ] Add breadcrumb navigation for interior pages
- [ ] Consider adding a Services page

#### SEO & Meta
- [ ] Update meta descriptions for all pages
- [ ] Add Open Graph images
- [ ] Create sitemap.xml
- [ ] Add structured data (JSON-LD) for local business

### Low Priority

#### Enhancements
- [ ] Add image gallery/lightbox for project photos
- [ ] Implement blog functionality for news/updates
- [ ] Add newsletter signup integration
- [ ] Consider adding before/after project comparisons
- [ ] Add video content support for project walkthroughs

#### Performance & Technical
- [ ] Optimize image loading and formats
- [ ] Implement lazy loading for below-fold images
- [ ] Add page transition animations
- [ ] Review and optimize bundle size

#### Accessibility
- [ ] Conduct full accessibility audit
- [ ] Test with screen readers
- [ ] Verify color contrast ratios
- [ ] Ensure keyboard navigation works throughout

---

## Known Issues

1. **Navigation Links:** Several navigation items point to template placeholder pages:
   - ~~"About" links to `/blog/`~~ FIXED - Now links to `/about/`
   - "Residential" links to `/accessibility-statement`
   - "Commercial" links to `/accessible-components`
   - "Civic" links to `/color-contrast-checker`

2. **Duplicate Images:** Tab panels all use the same placeholder image (`garden-2-small.jpg`)

3. **Hardcoded Typeform Link:** CallToAction component has a specific Typeform URL that may need updating

4. **Stats Numbers:** Counter values (900+, 25K+, etc.) are placeholder values that should be verified

---

## File Structure Reference

```
src/
├── assets/
│   ├── images/
│   │   └── landscape/
│   │       ├── garden-1-small.jpg
│   │       └── garden-2-small.jpg
│   └── scss/
├── components/
│   ├── BlockQuote.astro
│   ├── BreakoutImage.astro
│   ├── CallToAction.astro
│   ├── ColorContrast.astro
│   ├── ContentMedia.astro
│   ├── Counter.astro
│   ├── ExternalLink.astro
│   ├── ExternalLinkSocial.astro
│   ├── Feature.astro
│   ├── Footer.astro
│   ├── Header.astro
│   ├── Hero.astro
│   ├── Logo.astro
│   ├── Navigation.astro
│   ├── PageHeader.astro
│   ├── ResponsiveToggle.astro
│   ├── SiteMeta.astro
│   └── SocialShares.astro
├── content/
│   └── projects/
│       └── project-01.mdx ... project-07.mdx
├── layouts/
│   ├── DefaultLayout.astro
│   └── MarkdownLayout.astro
├── pages/
│   ├── index.astro (Homepage)
│   ├── about.astro (About Page)
│   ├── 404.astro
│   ├── accessibility-statement.astro
│   ├── accessible-components.astro
│   ├── color-contrast-checker.astro
│   ├── markdown-page.md
│   ├── blog/
│   │   ├── [...page].astro
│   │   └── [post].astro
│   └── portfolio/
│       ├── [...page].astro
│       └── [project].astro
└── styles/
```

---

## External Links & Resources

- **Live Form:** https://form.typeform.com/to/Gqmo3i
- **Houzz Profile:** https://www.houzz.com/pro/karenaitkenassociates/karen-aitken-and-associates
- **Instagram:** https://www.instagram.com/karenaitkenassociates/
- **Facebook:** https://www.facebook.com/KarenAitkenAssociates/
- **YouTube:** https://www.youtube.com/@karenaitkenassociates-land8166

---

## Notes

- This project is based on the [Accessible Astro Starter](https://github.com/incluud/accessible-astro-starter) template
- Uses `accessible-astro-components` library for UI components
- Primary font: Atkinson Hyperlegible for accessibility
- Color system uses OKLCH with automatic palette generation
