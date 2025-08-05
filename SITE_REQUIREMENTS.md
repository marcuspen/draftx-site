# DraftX Website Requirements for GitHub Pages

## Overview
Create a simple static website for DraftX using GitHub Pages. The site needs to serve as both a marketing landing page and support resource for the iOS app.

## Repository Setup
- Repository: `draftx-site` (already cloned)
- URL will be: https://draftx.football

## Required Pages

### 1. Landing Page (index.html)
**Purpose**: Marketing page to promote the app

**Required Sections**:
- Hero section with app logo and tagline: "5-a-side EPL Fantasy draft"
- Key features (use content from app_store_description.txt):
  - Position-specific scoring
  - 25+ tracked stats
  - Simple 5-a-side format
  - Live match updates
  - Fair draft system
- How it works (3-4 steps):
  1. Create or join a league
  2. Draft your 5-player squad
  3. Earn points based on real match performance
  4. Compete with friends
- Screenshot gallery - you can see at `./DraftX-Screens`
- Download buttons:
  - App Store button (link to app when live)
  - Google Play Store button (link to app when live)
- Footer with links to Support, Privacy Policy, Terms of Service

### 2. Support Page (support.html or /support/index.html)
**Purpose**: Help users and meet App Store requirements

**Required Sections**:
- FAQ Section covering:
  - How to create a league
  - How to join a league with invite code
  - How scoring works
  - How to make transfers
  - What happens if a player doesn't play
  - How the draft order works
- Scoring Guide:
  - Table showing position-specific scoring from ./scoring_groups.yaml
  - Explanation of why certain positions earn different points from other positions
- Contact Section:
  - Email: support@draftx.app
  - Contact form (can use Formspree or similar service)
- Links to Privacy Policy and Terms of Service

### 3. Privacy Policy (privacy.html)
**Purpose**: Required by App Store

Copy from /Users/marcus/personal_projects/draftx-platform/draftx-client/app/privacy-policy.tsx

### 4. Terms of Service (terms.html)
**Purpose**: Required by App Store

Copy from /Users/marcus/personal_projects/draftx-platform/draftx-client/app/terms-of-service.tsx

## Technical Requirements

### GitHub Pages Setup
1. Enable GitHub Pages in repository settings
2. Set source to main branch, root folder
3. Add CNAME file if using custom domain

### Recommended Structure
```
/
├── index.html
├── support.html
├── privacy.html
├── terms.html
├── CNAME (if using custom domain)
├── css/
│   └── styles.css
├── images/
│   ├── logo.png
│   ├── app-icon.png
│   ├── screenshots/
│   │   ├── screenshot1.png
│   │   ├── screenshot2.png
│   │   └── screenshot3.png
│   └── app-store-badge.svg
└── js/
    └── scripts.js (if needed)
```

### Design Guidelines
- Clean, modern design
- Mobile-responsive (many users will visit from phones)
- Fast loading (optimize images)
- Match app aesthetics if possible
- Use colors scheme from app is /Users/marcus/personal_projects/draftx-platform/draftx-client/constants/Colors.ts

### SEO Optimization
- Add meta tags for description, keywords
- Open Graph tags for social sharing
- Structured data for app information
- Sitemap.xml

### Content to Copy
Use content from `./app_store_description.txt` for:
- App description
- Feature lists
- Keywords for meta tags
- USP points

## Quick Start Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DraftX - 5-a-side Fantasy Premier League</title>
    <meta name="description" content="Draft your dream 5-a-side team! DraftX rewards smart tactics with position-specific scoring.">
    <meta name="keywords" content="fantasy,premier league,5-a-side,football,EPL,draft,soccer,FPL">
    <!-- Add CSS -->
</head>
<body>
    <!-- Content here -->
</body>
</html>
```

## Deployment Checklist
- [ ] All pages created and tested
- [ ] Mobile responsive design verified
- [ ] Images optimized for web
- [ ] Links all working
- [ ] Contact form tested
- [ ] GitHub Pages enabled
- [ ] Custom domain configured (if applicable)
- [ ] SSL certificate active (automatic with GitHub Pages)

## Notes
- Keep it simple - this is a support/marketing site, not a web app
- Focus on clear communication of the app's unique value proposition
- Ensure fast loading times
- Make support information easy to find
