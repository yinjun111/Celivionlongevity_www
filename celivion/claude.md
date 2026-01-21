# Celivion Longevity Website - Design Summary

## Overview
A modern, professional wellness and longevity website built with HTML, CSS, and JavaScript. The site promotes NAD+ therapies and wellness services under the Celivion brand.

## Branding Strategy

### Navigation
- **Logo/Brand Name**: "Celivion" (displayed in navigation bar, top left)
- **Content References**: "NAD+" (used throughout page content)

This dual-branding approach maintains Celivion as the company identity while emphasizing NAD+ as the core service offering.

## Website Structure

### Pages
1. **index.html** - Home page (React-based)
   - Title: "Celivion Longevity"
   - Features navigation bar overlay on React app

2. **about.html** - About Us
   - Company mission and approach
   - Why choose us section
   - Medical expertise highlights

3. **services.html** - Services
   - NAD+ IV Therapy
   - NAD+ Injections
   - Longevity Protocol
   - Medical Aesthetics

4. **membership.html** - Membership Plans
   - Essential ($299/month)
   - Premium ($799/month)
   - Elite ($1,499/month)

5. **contact.html** - Contact Us
   - Contact form
   - Location information

6. **login.html** - Member Login
   - Login form for existing members

## Navigation Design

### Fixed Navigation Bar
- Position: Fixed at top of viewport
- Background: White with subtle border
- Z-index: 9999 (ensures visibility over content)
- Box shadow for depth

### Navigation Links
- About Us → about.html
- Services → services.html
- Membership → membership.html
- Contact Us → contact.html
- LOGIN (button style) → login.html

### Styling
- Font: Inter (sans-serif)
- Link style: Uppercase, letter-spacing: 0.2em
- Color scheme:
  - Links: #52525b (zinc-600)
  - Brand: #18181b (zinc-950)
  - Login button: White text on #18181b background
- Responsive layout with flexbox

## Technical Details

### Index Page (Special Case)
- Built with React (script.js)
- Navigation bar added as static HTML overlay
- Uses inline styles with !important flags to ensure visibility
- Higher z-index to overlay React content

### Other Pages
- Standard HTML with Tailwind CSS classes
- Consistent navigation across all pages
- Current page highlighted with darker text color

### Server
- Python HTTP server running on port 8000
- Serves from /celivion directory
- Command: `python3 -m http.server 8000`

## Color Palette
- **Primary Dark**: #18181b (zinc-950)
- **Text Gray**: #52525b (zinc-600)
- **Light Gray**: #e4e4e7 (zinc-200)
- **Background**: White (#ffffff)
- **Accent**: #f4f4f5 (zinc-50)

## Typography
- **Primary Font**: Inter
- **Weights**: 300, 400, 500, 600, 700
- **Style**: Clean, modern, professional
- **Navigation**: Uppercase with wide letter spacing

## Design Principles
1. **Minimalist**: Clean, uncluttered layouts
2. **Professional**: Medical/wellness aesthetic
3. **High-end**: Premium feel matching luxury service offering
4. **Consistent**: Unified navigation and branding across all pages
5. **Accessible**: Clear hierarchy and readable typography

## File Structure
```
celivion/
├── index.html          # Home page (React app)
├── about.html          # About Us
├── services.html       # Services listing
├── membership.html     # Membership tiers
├── contact.html        # Contact form
├── login.html          # Member login
├── styles.css          # Global styles
└── script.js           # React app (minified)
```

## Recent Changes (Latest Commit)
- Added navigation bar to index.html
- Created new pages: about, contact, login, membership, services
- Implemented Celivion/NAD+ dual branding
- Updated page title to "Celivion Longevity"
- Removed server.log file

## Development Notes
- Navigation uses relative paths for proper server routing
- React app on index.html requires special handling for navigation overlay
- Hard browser refresh may be needed after updates due to caching
- All pages maintain consistent design language and navigation structure
