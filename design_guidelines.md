# Personal Portfolio Website Design Guidelines

## Design Approach
**Reference-Based:** Drawing from Linear's typography precision, Notion's content structure, and modern portfolio best practices (Dribbble/Behance). The design prioritizes creating an immediate professional impression while maintaining excellent readability for detailed content.

## Core Design Principles
1. **Professional First Impression:** Strong hero with personality
2. **Scannable Content:** Clear hierarchy for resume and course sections
3. **Project-Centric:** Showcase work with impact
4. **Purposeful Space:** Each section serves a clear goal

---

## Typography System

**Primary Font:** Inter (Google Fonts) - clean, professional
**Accent Font:** None needed - maintain simplicity

**Type Scale:**
- Hero Title: text-5xl md:text-6xl lg:text-7xl, font-bold
- Section Headers: text-3xl md:text-4xl, font-bold
- Subsection Headers: text-xl md:text-2xl, font-semibold
- Body: text-base md:text-lg, leading-relaxed
- Small Text/Labels: text-sm, font-medium

---

## Layout System

**Spacing Units:** Tailwind units of 4, 6, 8, 12, 16, 20, 24
- Section padding: py-16 md:py-24
- Component spacing: space-y-8 md:space-y-12
- Card padding: p-6 md:p-8

**Container Strategy:**
- Full-width sections with inner max-w-6xl mx-auto px-4
- Content-heavy sections: max-w-4xl for optimal reading

---

## Section Structure & Layout

### 1. Hero Section (80vh)
- Large hero image background with gradient overlay
- Centered content: Name, tagline, 1-2 sentence bio
- CTA button with blur backdrop
- Scroll indicator at bottom

### 2. About/Bio Section
- Two-column layout (md:grid-cols-2): Professional photo left, extended bio right
- Mobile: single column, photo first
- Include personality, background, current focus (3-4 paragraphs)

### 3. Goals Section
- Single column, centered content (max-w-3xl)
- Timeline-style layout: Short-term → Medium-term → Long-term goals
- Each goal: Icon + Title + Description
- Vertical connector line between goals

### 4. Skills Section
- Three-column grid (grid-cols-1 md:grid-cols-2 lg:grid-cols-3)
- Skill cards: Category header + skill badges/pills
- Categories: Technical Skills, Tools & Frameworks, Soft Skills

### 5. Projects Gallery
- Two-column masonry grid (md:grid-cols-2)
- Project cards with hover elevation
- Each card: Image/screenshot, title, description, tech stack tags, GitHub + Live demo links
- Minimum 4-6 projects showcased

### 6. Course Learnings Section
- Accordion/expandable cards layout
- Each course: Course name header, institution, key learnings list (3-5 bullets), skills gained tags
- Grid layout (md:grid-cols-2) for multiple courses

### 7. Resume Section
- Split layout: Timeline left (education + experience), downloadable resume CTA right
- Timeline entries: Organization, role/degree, dates, 2-3 achievement bullets
- "Download PDF Resume" button prominently placed

### 8. Contact/Footer
- Two-column: Contact form left, info (email, social links, availability) right
- Social icons: LinkedIn, GitHub, Email, Twitter/X
- Footer: Copyright, quick navigation links

---

## Component Library

**Navigation:**
- Fixed header with links to sections (smooth scroll)
- Mobile: hamburger menu
- Logo/name left, navigation right

**Cards:**
- Rounded corners (rounded-xl)
- Subtle shadow (shadow-lg)
- Hover: slight elevation increase (hover:shadow-2xl transition-shadow)
- Padding: p-6 md:p-8

**Buttons:**
- Primary: Bold text, generous padding (px-8 py-3), rounded-lg
- Buttons on images: backdrop-blur-md with semi-transparent background
- No custom hover states - rely on Button component

**Tags/Badges:**
- Pill shape (rounded-full px-4 py-1.5)
- Small text (text-sm)
- Used for skills, tech stack

**Form Inputs:**
- Consistent border-2, rounded-lg, p-3
- Focus states with ring effects

---

## Images

**Hero Background:**
- Professional workspace, coding setup, or abstract tech-themed image
- Gradient overlay for text readability
- Full bleed, positioned center

**About Section Photo:**
- Professional headshot or casual portrait
- Rounded-lg or rounded-full
- Size: 300-400px square

**Project Screenshots:**
- Actual project screenshots or mockups
- 16:9 or 3:2 aspect ratio
- High quality, clearly showing interface

---

## Animation Strategy
**Minimal approach:**
- Smooth scroll navigation only
- Subtle hover elevations on cards
- No scroll-triggered animations
- Focus on content, not motion

---

## Accessibility
- Semantic HTML throughout
- Proper heading hierarchy (h1 → h6)
- Alt text on all images
- Focus visible states on interactive elements
- ARIA labels for icon-only buttons