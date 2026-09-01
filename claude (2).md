# CLAUDE.md — Portfolio Dashboard

## Overview

Cyberpunk/futuristic themed portfolio dashboard. Plain HTML/CSS/JS — no framework,
no build step. Uses Poppins + Inter + JetBrains Mono fonts with glassmorphism effects.

## Files

- `index (1).html` — Redirects to dashboard.html immediately
- `dashboard.html` — Primary portfolio dashboard
- `dashboard (1).html` — Duplicate dashboard (must stay in sync)
- `photo-placeholder.jpg` — Profile photo (used as favicon + profile picture)

## Design System

- **Fonts:** Poppins (headings/buttons), Inter (body), JetBrains Mono (mono)
- **Colors (CSS variables):**
  - `--bg: #0a0a0f` — page background (near black)
  - `--surface: rgba(15,20,35,0.85)` — card/glass background
  - `--pink: #ff2d95` — primary neon accent (magenta)
  - `--cyan: #00e5ff` — secondary neon accent (cyan/blue)
  - `--violet: #8b5cf6` — orb gradient
  - `--green: #39ff14` — success/online indicator
  - `--amber: #f59e0b` — warning/beta indicator
  - `--text: #e8ecf3`, `--muted: #5a6d94`, `--faint: #3a4a6b`
  - `--border: rgba(0,229,255,0.1)` — glass border
- **Light Theme:** `.light` class swaps to light colors

## Dashboard Layout (dashboard.html)

### Topbar
- Hamburger menu (mobile)
- "ALI DEVELOPER" logo (ALI white, DEVELOPER pink)
- Search bar with dropdown (32 searchable items)
- Dark/Light mode toggle
- Notification bell with badge + dropdown (4 notifications)
- LOG OUT button (redirects to index (1).html)
- Profile picture with name/role

### Sidebar
- 9 nav items: Dashboard, About Me, Skills, Projects, Experience, Education, Certificates, Contact, GitHub Projects
- Active item highlighted with pink glow
- Social icons: GitHub, LinkedIn, Instagram
- Mobile: slide-in with overlay

### Main Content Sections

#### Dashboard (sec-dashboard)
- Profile card with photo, name, role, stats (50+ Projects, 1+ Years Exp, 10+ Tech, 100% Dedication)
- Terminal card with developer info JSON
- Skills Overview: 6 circular progress rings (HTML 95%, JS 90%, React 85%, Responsive 90%, AI 85%, API 80%)
- Recent Projects: 3 GitHub project cards (Mezban Restaurant, eBay Portfolio, Premium Pencil Selling)
- Quick Actions: 6 icon grid cards (About Me, Experience, Contact, Education, Certificates, GitHub)

#### About Me (sec-about)
- Full bio with premium stats row (1+ Year, 50+ Projects, 10+ Tech, 100% Dedication)
- 6 skill cards with colored icons (pink/cyan/violet/green/amber)

#### Skills (sec-skills)
- 8 detailed skill cards with descriptions + progress bars

#### Projects (sec-projects)
- 3 project cards with full descriptions

#### Experience (sec-experience)
- Premium timeline with glowing dots and gradient connecting line
- 2 jobs (Remote Web Developer + Office Clerk)
- Responsibility mini-cards in 2-column grid
- Colored skill badges

#### Education (sec-education)
- 3 premium glass cards:
  - Software Engineering (VU Lahore) - 2026-Present - Ongoing
  - ICS (Physics) - Punjab College Okara - 2023-2025 - Completed
  - Matric (Science) - Govt Boys High School - 2021-2023 - Completed

#### Certificates (sec-certificates)
- Premium "Total: 2" badge in header
- 2 large glass cards (cert-cards-grid, 2-column layout)
- Each card contains:
  - Icon with colored background (pink/violet)
  - Title + organization name
  - Meta row: Date, Duration, Verified badge
  - Gradient divider line
  - Description text
  - Skills title + 4 skill badges (HTML5, CSS3, JavaScript, etc.)
- Hover effects: lift + glow
- Responsive: 2→1 columns on mobile

#### Contact (sec-contact)
- Premium "Get In Touch" header with subtitle
- 6 premium contact cards in 2-column grid:
  - Phone (Pink) - Call Now button
  - Email (Cyan) - Send Mail button
  - LinkedIn (Violet) - Connect button
  - GitHub (Green) - Follow button
  - Instagram (Pink) - Follow button
  - Location (Cyan) - View Map button
- Availability card with green pulse dot:
  - Available for freelance work
  - Response time: Within 24 hours
  - Preferred: Email or LinkedIn

#### GitHub Projects (sec-github)
- Profile card with avatar, name, stats (8 repos, 4 stars, 14 followers, 49 following)
- 6 project cards with glassmorphism, language badges, GitHub links
- "View All on GitHub" gradient button

### Interactive Features
- All sidebar buttons navigate to corresponding sections
- Search bar filters through items and navigates on click
- Notification dropdown with mark all read
- Dark/Light theme toggle
- Count-up animation on stats
- Skill bars animate on scroll
- Scroll reveal animation on cards
- Profile image fallback (GitHub avatar → local photo-placeholder.jpg)

## Loading Screen

- Premium full-screen overlay with cyberpunk effects
- Gradient "ALI DEVELOPER" title with glitch flicker animation
- "// INITIALIZING SYSTEM..." subtitle with typing effect
- Animated progress bar (0-100%) with neon glow
- Status messages: "Loading modules...", "Initializing UI...", etc.
- Floating particles (pink, cyan, violet, green)
- Background grid overlay + scanline sweep
- Floating orbs (pink, cyan) with blur effect
- Auto-hides after progress reaches 100%

## Premium UI Components

### Glass Cards
- `backdrop-filter: blur(20px)`
- Semi-transparent backgrounds
- Subtle border with glow on hover
- Transform animations on hover

### Timeline (Experience)
- Vertical glowing line with dots
- Pulse animation on dots
- Glass cards with responsibility mini-cards

### Education/Certificate Cards
- Grid layout (2 columns)
- Colored icons with background
- Status badges (Ongoing/Completed/Verified)
- Subject/skill tags with colors

### Dashboard Skills
- Circular progress rings using conic-gradient
- 3-column grid layout
- Hover effects with transform

### Dashboard Projects
- GitHub-style cards with language badges
- Star count display
- External links to GitHub repos

### Quick Actions
- 3-column icon grid
- Colored icons with backgrounds
- Hover effects with transform

## Social Links

- GitHub: https://github.com/alee-pixel7
- LinkedIn: https://www.linkedin.com/in/aligohar-web
- Instagram: https://www.instagram.com/aleeeee__xo/

## Tawk.to Live Chat

- Embedded on dashboard.html
- Widget ID: `6a7486e8922c4f1d4a892c6b/1jvbitval`

## Contact Info

- Phone: 0324-4647704
- Email: rajputalee63@gmail.com

## Responsive Design

### Breakpoints
- **1024px**: Cards row, profile row, projects grid → 2 columns
- **768px**: Sidebar hides, hamburger shows, all grids adapt
- **520px**: Single column layout, smaller padding, compact cards
- **380px**: Ultra-compact for smallest phones

### Responsive Sections
- Topbar: Hamburger menu, search hides on mobile
- Sidebar: Slide-in with overlay
- Dashboard Cards: Single column
- Skills Overview: 3→2 columns
- Quick Actions: 3→2 columns
- About Me: 2→1 columns
- Experience Timeline: Adjusted layout
- Education Cards: 2→1 columns
- Certificates Cards: 2→1 columns
- Contact Premium: 2→1 columns
- GitHub Projects: 3→2→1 columns
- GitHub Profile: Stacked layout

## How to Run

No build step. Open `dashboard.html` in browser or use Live Server.
