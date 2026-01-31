# Tall Pups

A minimal static landing page for Tall Pups - "bored, not broken".

## Overview

This is a simple, single-page website deployed as a static site to Firebase Hosting. The site features a clean design with custom typography and a call-to-action linking to the Tall Pups merchandise store.

## Project Structure

```
.
├── public/
│   ├── index.html      # Main landing page
│   └── JennaSue.ttf    # Custom font file
├── firebase.json       # Firebase hosting configuration
├── .firebaserc        # Firebase project configuration
└── package.json       # Dependencies (Firebase SDK)
```

## Features

- **Zero build process**: Pure HTML with inline CSS
- **Custom typography**: Uses Jenna Sue font for branding
- **Responsive design**: Fluid typography with `clamp()` for all screen sizes
- **Centered layout**: Flexbox-based vertical and horizontal centering
- **Firebase hosting**: Configured for static file deployment

## Development

### Prerequisites

- Node.js (for local development server)
- Firebase CLI (for deployment)

### Local Development

To view the site locally, you can use any static file server:

**Option 1: Using npx serve**
```bash
npx serve public
```

**Option 2: Using Python's built-in server**
```bash
cd public
python3 -m http.server
```

**Option 3: Using Firebase emulator**
```bash
firebase emulators:start
```

The site will be available at `http://localhost:5000` (or the port shown in your terminal).

## Deployment

This site is deployed to Firebase Hosting.

### Prerequisites

1. Install Firebase CLI:
```bash
npm install -g firebase-tools
```

2. Login to Firebase:
```bash
firebase login
```

### Deploy to Production

```bash
firebase deploy
```

The site will be deployed to: `https://tallpups.web.app` (or your configured Firebase domain)

### Firebase Configuration

- **Project**: `tallpups`
- **Public directory**: `public/`
- **Single-page app**: All routes rewrite to `/index.html`

## Technical Details

### Styling

- **Typography**: Georgia (serif) for body text, Jenna Sue (custom) for title
- **Color scheme**: Black text on white background
- **Responsive text sizing**: Using CSS `clamp()` for fluid scaling
- **Layout**: Centered flexbox with vertical stacking

### Font Loading

The custom Jenna Sue font uses `font-display: swap` for optimal loading performance and to prevent FOUT (Flash of Unstyled Text).

## License

All rights reserved.
