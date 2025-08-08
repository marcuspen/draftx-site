# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview
DraftX is a static website for a 5-a-side Fantasy Premier League mobile app, hosted on GitHub Pages. The site serves as both a marketing landing page and support resource.

## Project Structure
- Static HTML site with vanilla JavaScript (no build process required)
- Main pages: `index.html`, `support.html`, `scoring.html`, `privacy.html`, `terms.html`
- CSS styling in `css/styles.css`
- JavaScript functionality in `js/scripts.js`
- Position-specific scoring data in `scoring_groups.yaml`

## Development Commands
Since this is a static site with no build process:
- **Local development**: Open `index.html` directly in browser or use a local server (e.g., `python -m http.server 8000`)
- **Deploy**: Push changes to main branch - GitHub Pages automatically deploys from root folder

## Key Architecture
- **Scoring System**: Position-specific points for 25+ stats tracked in `scoring_groups.yaml`
  - Different point values for GK, DEF, MID, FWD positions
  - Rewards position-appropriate actions (e.g., saves for GK, tackles for DEF)
- **Mobile-First Design**: Responsive CSS with mobile menu toggle
- **No Framework Dependencies**: Pure HTML/CSS/JS for fast loading and simplicity

## Important Context
- Site URL: https://draftx.football (configured via CNAME file)
- App details and features documented in `SITE_REQUIREMENTS.md`
- Screenshots located in `DraftX-Screens/` and `images/screenshots/`
- Contact email: support@draftx.football