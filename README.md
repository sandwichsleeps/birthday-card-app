# 🎉 Birthday Card Giggle Machine

A fun, lightweight **Progressive Web App (PWA)** that generates funny, printable birthday messages in seconds.

Users can create personalised birthday cards by entering a name, age, hobby, adjective, and plural noun.  
The app automatically adjusts tone by age, saves cards locally, works offline, and can be installed like a real mobile app.

🔗 **Live App**  
https://sandwichsleeps.github.io/birthday-card-app/

---

## ✨ Features

- 🎂 Generate funny, personalised birthday messages
- 🧠 Age-aware tone (kid / teen / adult / senior)
- 💾 Cards are **automatically saved locally**
- 🔗 Shareable links with pre-filled card data
- 🖨️ Printable card layout (print one card at a time)
- 📱 **Installable PWA** (iOS & Android)
- 🌐 Works **offline** once installed
- 🎨 Clean, playful UI with custom app icon
- ⚡ No frameworks, fast load, lightweight

---

## 📱 Install as an App

### iPhone (Safari)
1. Open the app link
2. Tap **Share**
3. Select **Add to Home Screen**

### Android (Chrome)
1. Open the app link
2. Tap **Install App** or **Add to Home screen**

Once installed, the app runs in standalone mode without a browser address bar.

---

## 🛠️ Tech Stack

- **HTML5**
- **CSS3** (responsive layout, gradients, modern UI)
- **Vanilla JavaScript**
- **Progressive Web App (PWA)**
  - Service Worker
  - Web App Manifest
  - Offline caching
- **LocalStorage** (persistent card storage)
- **GitHub Pages** (hosting)

No frameworks. No build tools. No backend.

---

## 📂 Project Structure

birthday-card-app/
├── index.html
├── manifest.webmanifest
├── service-worker.js
├── icons/
│ ├── icon-192.png
│ └── icon-512.png
└── README.md



---

## 🚀 How It Works

1. User enters card details (name, age, hobby, adjective, plural noun)
2. App generates a personalised birthday message
3. Tone is automatically adjusted based on age
4. Card is saved locally in the browser
5. Cards stack visually (newest first)
6. Users can:
   - Print a single card
   - Copy message text
   - Share a pre-filled link
   - Edit or delete saved cards
7. App continues to work offline via Service Worker cache

---

## 🔄 Updating the App (PWA Cache)

When making changes to cached files (HTML, icons, etc.):

1. Open `service-worker.js`
2. Update the cache version:
   ```js
   const CACHE_VERSION = "bday-pwa-vX";

