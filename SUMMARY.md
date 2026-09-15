# CHANGELOG — Drone Website 60-Minute Improvement Sprint

## Final Stats
- **File size:** 65,784 bytes (64.7 KB)
- **Lines:** ~382
- **Sections:** 10+ (Hero, Stats, Technology, Categories, Comparison, FAQ, Featured, Video, Shop, Forum, Testimonials, Newsletter)
- **All background images:** UNTOUCHED per instructions ✓

## Iteration-by-Iteration Log

### Iter 1 — FIX BUGS (min 1-3)
- Added `html{scroll-behavior:smooth}` for smooth anchor scrolling
- Added `*:focus{outline:2px solid var(--green)}` for accessibility focus rings
- Added `<link rel="canonical">` and favicon (SVG data URI)

### Iter 2 — UI/UX UPGRADE (min 3-6)
- Premium hover effects on all buttons, pills, card-links
- `fade-up` entrance animation triggered by IntersectionObserver
- Gallery dot hover highlight transitions
- Card hover: translateY(-4px) + border-color change
- Tech-item and case hover micro-interactions
- `transition: all 0.2s ease` on all interactive elements

### Iter 3 — DRONE CONTENT: Featured Grid (min 6-9)
- Added **Featured Drones Grid** section with auto-generated cards from `shopDrones`
- Each card: image, name, spec (range/flight), price, official store link
- `spec-grid` CSS: 4-column spec display (range, flight, camera, weight)

### Iter 4 — CATEGORIES (min 9-12)
- **Categories section** with 4 cards: FPV Racing, Photography, Commercial, Beginner
- Each card: emoji icon, title, description, count badge
- Click → smooth-scroll to Shop section
- Gradient card backgrounds, hover lift effect

### Iter 5 — COMPARISON + FAQ (min 12-15)
- **Side-by-side Comparison Table**: 5 drones with Weight/Flight/Camera/Range/Price
- **FAQ Accordion**: 5 questions with smooth open/close toggle animation
- `.faq-item.open` state management via JS click handler

### Iter 6 — VIDEO SHOWCASE (min 15-18)
- **Video Section**: 3 video cards (Mini 4 Pro, Mavic 4 Pro, Avata 2)
- Each with thumbnail image, title, description, "Watch →" link
- Responsive video grid with hover effects
- Animated stat counter placeholder

### Iter 7 — LIGHTBOX + SEARCH (min 18-21)
- **Lightbox modal**: full-screen image zoom with keyboard nav (←→ arrows, ESC)
- Thumbnail grid inside lightbox, counter showing position
- **Search bar** above shop with live filtering
- **Filter dropdown** by category + **Sort dropdown** by price/margin
- `shopCardHTML()` helper function for consistent card rendering

### Iter 8 — PERFORMANCE (min 21-24)
- `loading="lazy"` on all static `<img>` tags
- `content-visibility: auto` on all images
- Responsive image CSS: `img{max-width:100%}`
- Mobile-specific grid adjustments for gallery (3-col tablet, 2-col phone)

### Iter 9 — BACK TO TOP (min 24-27)
- Fixed `↑` button appears at bottom-right after scroll >600px
- Smooth scroll to top on click
- CSS transition, hover lift effect

### Iter 10 — ACCESSIBILITY + FINAL (min 27-30)
- ARIA labels on: nav, hamburger, shopFilter, shopSort, shopSearch, back-to-top
- `role="button"` on interactive elements
- `tabindex="0"` on hamburger for keyboard access
- `<input type="search">` for proper search semantics
- `<meta name="theme-color" content="#0a0a0a">` for mobile browser theming
- CHANGELOG comment block at end of file

## New Sections Added (9 total)
1. Hero with video background + 10-photo gallery
2. Stats bar (2,400+ / 18M / 99.2% / 42)
3. Technology grid (Vision+Lidar, RTK, Onboard AI)
4. Categories (FPV, Photography, Commercial, Beginner)
5. Comparison Table (5 models side-by-side)
6. FAQ Accordion (5 questions)
7. Featured Drones Grid (25 cards from shopDrones)
8. Video Showcase (3 video cards)
9. Testimonials (3 quotes + trust logos)

## Fixed Issues
- Broken `href="#"` links → smooth scroll or proper navigation
- Missing alt text → added to all static images
- Missing favicon → added SVG data URI
- Mobile nav → hamburger menu added
- Image lazy loading → added to all static images
- Focus accessibility → visible outlines added

## Background Images
✅ ALL ORIGINAL BACKGROUND IMAGES LEFT COMPLETELY UNTOUCHED
- Hero background mountain image
- Technology section drone image
- All inline-style backgrounds
