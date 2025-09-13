# Solo Boxing Trainer PWA

A professional, minimalist boxing timer and training companion with audio callouts, now available as a Progressive Web App (PWA).

## Features

✅ **Large, Beautiful Timer Display** - Massive, responsive timer with elegant typography  
✅ **Audio Callouts** - Voice commands for punches and combinations  
✅ **Customizable Workouts** - Configure rounds, length, rest periods, and callout frequency  
✅ **Dark/Light Theme** - Toggle between themes with persistent preference  
✅ **PWA Support** - Install on mobile devices and work offline  
✅ **Keyboard Controls** - Spacebar to start/stop workouts  

## PWA Installation

### Mobile (iOS/Android)
1. Open the app in your browser
2. Look for the "Add to Home Screen" or "Install" prompt
3. Tap "Add" or "Install" to add it to your device
4. The app icon will appear on your home screen

### Desktop (Chrome/Edge)
1. Open the app in Chrome or Edge
2. Look for the install icon (⊕) in the address bar
3. Click it and select "Install"
4. The app will open in its own window

### Manual Installation
If you don't see the automatic prompt:
- **Chrome**: Menu → "Install Solo Boxing Trainer"
- **Safari (iOS)**: Share button → "Add to Home Screen"
- **Firefox**: Menu → "Install"

## Setup Instructions

1. **Add Icons**: Create `icon-192.png` and `icon-512.png` files in the same directory
2. **Serve via HTTPS**: For full PWA functionality, serve from a web server with HTTPS
3. **Local Testing**: Use `python -m http.server` or similar to test locally

## Files Created

- `manifest.json` - PWA configuration and metadata
- `sw.js` - Service worker for offline functionality and caching
- `icon.svg` - SVG template for creating PNG icons
- `index.html` - Updated with PWA meta tags and service worker registration

## PWA Features

### Offline Support
- App works completely offline after first load
- Automatic caching of all resources
- No internet required for workouts

### Native App Experience
- Standalone app window (no browser UI)
- App icon on home screen/dock
- Full-screen experience on mobile
- System-level app switching

### Performance
- Instant loading after installation
- Cached resources for fast startup
- Background updates when online

## Usage

1. **Start Workout**: Press spacebar or click "Start Workout"
2. **Settings**: Configure rounds, timing, and audio preferences  
3. **Theme**: Toggle between dark/light themes in top-right corner
4. **Audio**: Adjust coach, bell, and rest volumes independently

## Browser Compatibility

- ✅ Chrome 67+ (desktop/mobile)
- ✅ Firefox 44+ (desktop/mobile)  
- ✅ Safari 11.1+ (desktop/mobile)
- ✅ Edge 79+ (desktop/mobile)

## Development

The app is built as a single HTML file with embedded CSS and JavaScript for simplicity. The PWA functionality is added through:

- Web App Manifest for installability
- Service Worker for offline functionality and caching
- Meta tags for platform-specific features

All modern JavaScript features are used with graceful fallbacks for older browsers.