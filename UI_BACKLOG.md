# UI Backlog - KAA Landing

A prioritized list of user interface improvements and new features for the Karen Aitken & Associates landing page.

---

## Backlog Overview

| Priority | Count | Description |
|----------|-------|-------------|
| High     | 6     | Critical for user experience and conversions |
| Medium   | 8     | Enhances functionality and engagement |
| Low      | 5     | Nice-to-have improvements |

---

## High Priority

### 1. Contact Form Integration
- **Status:** To Do
- **Description:** Replace external Typeform link with a native contact form component
- **Acceptance Criteria:**
  - [ ] Form fields: Name, Email, Phone, Project Type, Message
  - [ ] Client-side validation with accessible error messages
  - [ ] Form submission handling (Netlify Forms, Formspree, or API)
  - [ ] Success/error state feedback
  - [ ] Keyboard accessible with proper focus management
- **Components:** New `ContactForm.astro`

### 2. About Page
- **Status:** To Do
- **Description:** Create a dedicated About page showcasing the firm's story, values, and team
- **Acceptance Criteria:**
  - [ ] Company history and mission statement
  - [ ] Team member profiles with photos
  - [ ] Design philosophy section
  - [ ] Awards/recognition display
  - [ ] Responsive layout matching site design
- **Components:** New page `src/pages/about.astro`, possibly `TeamMember.astro`

### 3. Services Pages
- **Status:** To Do
- **Description:** Individual pages for each service offering (Residential, Commercial, Civic)
- **Acceptance Criteria:**
  - [ ] Service overview with key benefits
  - [ ] Process/workflow visualization
  - [ ] Related portfolio projects
  - [ ] Service-specific CTAs
  - [ ] Consistent navigation between services
- **Components:** `src/pages/services/[service].astro` or individual pages

### 4. Portfolio Gallery Enhancements
- **Status:** To Do
- **Description:** Improve portfolio browsing experience with filtering and lightbox
- **Acceptance Criteria:**
  - [ ] Category/tag filtering (Residential, Commercial, etc.)
  - [ ] Lightbox modal for full-size image viewing
  - [ ] Keyboard navigation in lightbox (arrow keys, escape)
  - [ ] Image zoom capability
  - [ ] Touch-friendly swipe gestures
- **Components:** `GalleryLightbox.astro`, `PortfolioFilter.astro`

### 5. Mobile Navigation Improvements
- **Status:** To Do
- **Description:** Enhance mobile menu experience and touch interactions
- **Acceptance Criteria:**
  - [ ] Smooth slide-in animation for mobile menu
  - [ ] Touch-friendly tap targets (min 44px)
  - [ ] Backdrop overlay when menu is open
  - [ ] Focus trap within open menu
  - [ ] Close on outside tap or swipe
- **Components:** Update `Navigation.astro`, `ResponsiveToggle.astro`

### 6. Testimonial Carousel
- **Status:** To Do
- **Description:** Display multiple client testimonials in a rotating carousel
- **Acceptance Criteria:**
  - [ ] Auto-advance with pause on hover/focus
  - [ ] Manual navigation controls (prev/next, dots)
  - [ ] Keyboard accessible navigation
  - [ ] Screen reader announcements for slide changes
  - [ ] Touch swipe support
  - [ ] Reduced motion preference respected
- **Components:** `TestimonialCarousel.astro`

---

## Medium Priority

### 7. Before/After Image Slider
- **Status:** To Do
- **Description:** Interactive slider to compare project transformations
- **Acceptance Criteria:**
  - [ ] Draggable divider between before/after images
  - [ ] Touch and mouse support
  - [ ] Keyboard controls (arrow keys)
  - [ ] Labels for before/after states
  - [ ] Works at various viewport sizes
- **Components:** `BeforeAfterSlider.astro`

### 8. Project Timeline Component
- **Status:** To Do
- **Description:** Visual timeline showing the design process phases
- **Acceptance Criteria:**
  - [ ] Vertical/horizontal orientation options
  - [ ] Phase markers with descriptions
  - [ ] Current phase highlighting
  - [ ] Animated reveal on scroll
  - [ ] Responsive design
- **Components:** `ProcessTimeline.astro`

### 9. Newsletter Signup
- **Status:** To Do
- **Description:** Email subscription form for garden tips and updates
- **Acceptance Criteria:**
  - [ ] Email input with validation
  - [ ] Integration with email service (Mailchimp, ConvertKit)
  - [ ] Success/error feedback
  - [ ] Optional placement in footer and/or popup
  - [ ] GDPR-compliant consent checkbox
- **Components:** `NewsletterSignup.astro`

### 10. Client Logo Grid
- **Status:** To Do
- **Description:** Display logos of notable clients or partners
- **Acceptance Criteria:**
  - [ ] Responsive grid layout
  - [ ] Grayscale with color on hover
  - [ ] Alt text for accessibility
  - [ ] Optional link to case study
  - [ ] Animation on scroll into view
- **Components:** `ClientLogos.astro`

### 11. Floating CTA Button
- **Status:** To Do
- **Description:** Persistent call-to-action button for quick contact access
- **Acceptance Criteria:**
  - [ ] Fixed position (bottom-right corner)
  - [ ] Appears after scrolling past hero
  - [ ] Subtle entrance animation
  - [ ] Does not obstruct content
  - [ ] Hides when footer is visible
- **Components:** `FloatingCTA.astro`

### 12. FAQ Enhancements
- **Status:** To Do
- **Description:** Improve existing FAQ accordion with search and categories
- **Acceptance Criteria:**
  - [ ] Search/filter functionality
  - [ ] Category grouping
  - [ ] Expand all/collapse all buttons
  - [ ] Deep linking to specific questions
  - [ ] Schema markup for SEO
- **Components:** Update existing FAQ section, add `FAQSearch.astro`

### 13. Blog Category Pages
- **Status:** To Do
- **Description:** Category and tag pages for blog organization
- **Acceptance Criteria:**
  - [ ] Category listing page
  - [ ] Posts filtered by category
  - [ ] Tag cloud component
  - [ ] Related posts suggestions
  - [ ] Breadcrumb navigation
- **Components:** `src/pages/blog/category/[category].astro`, `TagCloud.astro`

### 14. Loading States & Skeleton Screens
- **Status:** To Do
- **Description:** Add loading indicators for dynamic content
- **Acceptance Criteria:**
  - [ ] Skeleton placeholders for images
  - [ ] Loading spinners for form submissions
  - [ ] Smooth content reveal animations
  - [ ] Reduced motion alternatives
- **Components:** `Skeleton.astro`, `LoadingSpinner.astro`

---

## Low Priority

### 15. Dark Mode Toggle Enhancement
- **Status:** To Do
- **Description:** Improve dark mode toggle with system preference sync
- **Acceptance Criteria:**
  - [ ] Three-way toggle (light/dark/system)
  - [ ] Smooth transition between modes
  - [ ] Persist preference in localStorage
  - [ ] Icon change animation
- **Components:** Update theme toggle in `Header.astro`

### 16. Print Stylesheet
- **Status:** To Do
- **Description:** Optimized styles for printing pages
- **Acceptance Criteria:**
  - [ ] Hide navigation, footer, and interactive elements
  - [ ] Optimize images for print
  - [ ] Add URL display for links
  - [ ] Proper page breaks
- **Components:** `_print.scss`

### 17. 404 Page Enhancement
- **Status:** To Do
- **Description:** Make the error page more helpful and branded
- **Acceptance Criteria:**
  - [ ] Search functionality
  - [ ] Suggested pages/popular links
  - [ ] Illustration or branded imagery
  - [ ] Clear navigation back to home
- **Components:** Update `src/pages/404.astro`

### 18. Social Sharing Buttons
- **Status:** To Do
- **Description:** Add share buttons for blog posts and projects
- **Acceptance Criteria:**
  - [ ] Share to Twitter, Facebook, LinkedIn, Pinterest
  - [ ] Copy link functionality
  - [ ] Accessible button labels
  - [ ] Open Graph preview optimization
- **Components:** `SocialShare.astro`

### 19. Scroll Progress Indicator
- **Status:** To Do
- **Description:** Visual indicator showing page scroll progress
- **Acceptance Criteria:**
  - [ ] Horizontal bar at top of page
  - [ ] Smooth animation
  - [ ] Matches brand colors
  - [ ] Optional per-page enable/disable
- **Components:** `ScrollProgress.astro`

---

## Completed

_Items will be moved here as they are completed._

---

## Notes

### Design Guidelines
- All components must meet WCAG 2.1 AA accessibility standards
- Follow existing OKLCH color system (primary: #00aad1, secondary: #00e11e)
- Maintain Atkinson Hyperlegible font for readability
- Respect reduced motion preferences
- Mobile-first responsive design

### Component Standards
- Use Astro components (`.astro` files)
- Follow existing naming conventions
- Include TypeScript prop interfaces where appropriate
- Document component usage with examples

### Testing Checklist
- [ ] Keyboard navigation
- [ ] Screen reader compatibility
- [ ] Color contrast (use built-in checker)
- [ ] Responsive breakpoints (mobile, tablet, desktop)
- [ ] Dark mode support
- [ ] Reduced motion mode

---

*Last updated: 2026-01-09*
