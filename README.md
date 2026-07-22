# Training HQ — CrossFit & Lifting Log

A PWA (Progressive Web App) workout tracker for CrossFit and Olympic weightlifting.

## Features
- Workout log with RPE, energy, sets/reps/weight
- Personal Records board (seeded from Wodify history)
- Muscular Load radar chart + volume breakdown
- Movement library with PR badges
- Weekly training strip
- **Works offline** · **Installable on iPhone home screen**

## Deploy to Netlify (5 min)

1. Push this repo to GitHub
2. Go to [netlify.com](https://netlify.com) → **Add new site** → **Import from Git**
3. Select this repo
4. Build settings: leave blank (no build command needed)
5. Publish directory: `.` (root)
6. Click **Deploy site**

Netlify will give you a URL like `https://training-hq.netlify.app`

## Install on iPhone

1. Open the Netlify URL in Safari
2. Tap the **Share** button (box with arrow)
3. Scroll down → tap **Add to Home Screen**
4. Tap **Add**

The app will appear on your home screen with its own icon and launch fullscreen — no browser chrome.

## Data persistence

Workouts are saved to `localStorage` in your browser/app. They persist across sessions on the same device.

## Files

| File | Purpose |
|---|---|
| `index.html` | Full self-contained app (React + Recharts via CDN) |
| `manifest.json` | PWA metadata (name, icon, display mode) |
| `sw.js` | Service worker for offline support |
| `icon-192.png` | App icon (home screen) |
| `icon-512.png` | App icon (splash screen) |
