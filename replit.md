# Grow a Garden Pet Giveaway Website

## Overview

This is a static website for a Roblox "Grow a Garden" game pet giveaway system. The site provides a modern, dark-themed interface where users can browse available pets and request them for free. Built with pure HTML, CSS, and JavaScript, it's designed to be lightweight and easily deployable on GitHub Pages.

## System Architecture

### Frontend Architecture
- **Single Page Application (SPA)**: The entire application is contained in a single `index.html` file
- **Vanilla JavaScript**: No complex frameworks, using pure JS for interactivity
- **Bootstrap 5**: For responsive grid system and UI components
- **Font Awesome 6**: For icons and visual elements
- **CSS Custom Properties**: Modern CSS variables for consistent theming

### Static Site Design
- **No Backend Required**: All functionality is client-side
- **GitHub Pages Deployment**: Automated deployment through GitHub Actions
- **Mobile-First Responsive**: Designed to work on all device sizes

## Key Components

### 1. Pet Gallery System
- Visual card-based display for pets (160x160px images)
- Rarity badge system for pet classification
- Stock counter display
- Interactive pet selection

### 2. Theme System
- Dark theme with custom CSS variables:
  - Primary background: `#000000`
  - Card background: `rgba(42, 42, 42, 0.95)`
  - Accent colors: `#00d4ff` (blue), `#ff6b6b` (red)
  - Typography: Inter font family with fallbacks

### 3. Navigation & Layout
- Fixed navbar with smooth scrolling
- Responsive Bootstrap grid system
- Section-based content organization

## Data Flow

### Client-Side Only Architecture
1. **Page Load**: HTML loads with embedded CSS and JavaScript
2. **Pet Display**: Static pet data rendered as cards
3. **User Interaction**: JavaScript handles form submissions and UI state
4. **Contact System**: Links to external platforms (Discord/Roblox)

### No Database Integration
- Pet inventory is hardcoded in HTML
- No persistent data storage
- No user authentication system
- Contact handled through external platforms

## External Dependencies

### CDN Dependencies
- **Bootstrap 5.3.0**: UI framework and components
- **Font Awesome 6.0.0**: Icon library
- **Google Fonts (Inter)**: Typography

### External Platforms
- **Discord**: User communication
- **Roblox**: Game integration
- **GitHub Pages**: Hosting platform

## Deployment Strategy

### GitHub Pages Deployment
- **Source**: Deploy from main branch root directory
- **Automatic Deployment**: GitHub Actions workflow (`.github/workflows/deploy.yml`)
- **Static Hosting**: No server-side processing required
- **Custom Domain Support**: Available through GitHub Pages settings

### Development Workflow
1. Code changes pushed to main branch
2. GitHub Actions automatically deploys to Pages
3. Live site updates within minutes
4. No build process required (pure static files)

## Changelog

```
Changelog:
- June 29, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```

## Notes for Development

### Current Limitations
- No backend database (all data is static)
- No user authentication
- No real-time inventory management
- Contact system relies on external platforms

### Potential Enhancements
- Add a simple backend with database for dynamic inventory
- Implement user registration/login system
- Add real-time stock updates
- Create admin panel for pet management

### Security Considerations
- Currently no sensitive data handling
- All code is client-side and publicly visible
- External links should be validated before deployment