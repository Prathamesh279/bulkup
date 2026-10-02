# BulkUp – Indian Bulking Tracker

A lightweight offline-first PWA for tracking Indian home food calories & protein while bulking.

## Features
- Indian food database (roti, dal, paneer, eggs, biryani, sattu, etc.)
- Daily calorie & protein rings + quests
- Water tracker (3.5 L)
- Weight log + progress chart
- Custom foods, quick-add recent items
- XP / levels / streaks / badges
- Dark mode (follows system)
- **Installable** as an app on phone & desktop
- Works offline after first load

> **Note:** The AI plate-scan tab only works when the page is opened inside Claude (claude.ai). Everywhere else, use the Foods tab to log meals.

## How to use / install

### Option A – Phone (easiest)
1. Put the whole `bulkup` folder on any static host (GitHub Pages, Netlify, Vercel, Cloudflare Pages, or even a simple Python/HTTP server).
2. Open the site in **Chrome** (Android) or **Safari** (iPhone).
3. Install:
   - **Android Chrome:** menu → “Install app” / “Add to Home screen”
   - **iPhone Safari:** Share → “Add to Home Screen”
4. The app icon appears on your home screen and opens full-screen like a native app.

### Option B – Local (no internet needed after first open)
```bash
cd bulkup
python3 -m http.server 8080
```
Then open http://localhost:8080 on your phone (same Wi-Fi) or computer and install from the browser.

### Option C – Desktop
Open the site in Chrome/Edge → address bar install icon (or menu → Install BulkUp).

## Files
| File | Purpose |
|------|---------|
| `index.html` | The whole app |
| `manifest.webmanifest` | PWA install metadata |
| `sw.js` | Offline cache |
| `icon-192.png` / `icon-512.png` | App icons |
| `apple-touch-icon.png` | iOS home-screen icon |

All data is stored in your browser’s `localStorage` – nothing is sent to a server.

## Default profile
Starts at 48 kg, 170 cm, age 22, moderate activity, goal 55 kg, +500 kcal surplus. Change everything in the Progress tab.
