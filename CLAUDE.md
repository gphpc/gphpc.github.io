# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GitHub Pages website for "고척푸르지오힐스테이트 입주예정자협의회" (Gocheok Prugio Hill State Residents Council). It's a single-page application built using the HTML5 UP "Dimension" template with Korean localization.

## Architecture

**Frontend Framework**: Vanilla HTML/CSS/JavaScript with jQuery
- **Template**: HTML5 UP Dimension template
- **Styling**: SCSS preprocessor with modular component structure
- **JavaScript**: jQuery-based single-page application with hash-based routing
- **Layout**: Responsive design with mobile-first approach

**Key Components**:
- `index.html`: Main entry point with complete application structure
- `assets/sass/`: SCSS source files organized by components, layout, and base styles
- `assets/css/`: Compiled CSS files (main.css is compiled from SCSS)
- `assets/js/`: JavaScript modules for interactivity and responsive behavior
- `images/`: Static assets including favicons, icons, and background images

## Development Workflow

**SCSS Compilation**: 
- Source files are in `assets/sass/` with modular structure:
  - `base/`: Reset, typography, page fundamentals
  - `components/`: Reusable UI components (buttons, forms, icons, etc.)
  - `layout/`: Layout-specific styles (header, footer, main, wrapper)
  - `libs/`: Variables, mixins, functions, vendor imports
- SCSS must be compiled to `assets/css/main.css` for production
- No build system is currently configured - manual compilation required

**File Structure**:
- Static site served directly from repository root
- No server-side processing required
- Assets organized in conventional `assets/` directory structure

**Content Management**:
- All content is hardcoded in `index.html`
- Korean language content for apartment complex residents
- Navigation uses hash-based routing with jQuery animations
- External links to KakaoTalk, Naver Cafe, and consent forms

## Key Features

- **Single Page Application**: Hash-based routing with smooth transitions
- **Responsive Design**: Breakpoint-based layout (xxsmall to xlarge)
- **Korean Localization**: All content in Korean for local community
- **External Integrations**: Links to KakaoTalk chat rooms and Naver Cafe
- **Favicon System**: Complete favicon set for various devices and browsers

## Development Commands

Since this is a static site with no build system configured:

**SCSS Compilation** (manual):
```bash
# Install SASS globally if needed
npm install -g sass

# Compile SCSS to CSS
sass assets/sass/main.scss assets/css/main.css

# Watch for changes during development
sass --watch assets/sass/main.scss:assets/css/main.css
```

**Local Development**:
- Serve files using any static file server
- Python: `python -m http.server 8000`
- Node.js: `npx http-server`
- VS Code Live Server extension

**Testing**: No automated tests - manual browser testing required

## Important Notes

- The repository name suggests this was forked from "recrash.github.io" but is now used for "gphpc.github.io"
- Package.json exists but only includes Claude Code dependency - no build scripts defined
- CSS is pre-compiled and committed to repository
- All external links point to Korean services (KakaoTalk, Naver)
- Content is specific to apartment complex residents and入주예정자협의회 (prospective residents council)