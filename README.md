# 📱 Meenakshi Finance - வட்டி கணக்கிடும் பயன்பாடு

A **Tamil-first Progressive Web App (PWA)** for calculating loan/pawn (`அடகு`) interest.  
Designed to be **simple, mobile-friendly, and senior-citizen friendly**, with a fixed **1.25% monthly interest rate** and automatic calculations for **days, months, and years**.

---

## ✨ Features

- **Tamil UI** 🇮🇳 – All labels, hints, and error messages are in Tamil.  
- **Fixed Interest Rate** – Always **1.25% per month**, read-only.  
- **Friendly Date Input**  
  - Enter date in **DD/MM/YYYY** format (slashes auto-inserted as you type).  
  - Or pick from a **calendar**.  
  - Validates the date and blocks **future dates**.  
- **Auto “Today”** – Filled automatically and locked.  
- **Auto Day Count** – Days between start date and today are calculated automatically.  
- **Bold Duration Breakdowns**  
  - Example: `45 days → 1 மாதம் 15 நாள்` and `0 வருடம் 1 மாதம் 15 நாள்`.  
  - Displayed clearly for better visibility.  
- **Multiple Views (Always On)**  
  - Daily calculation.  
  - Monthly (30-day months).  
  - Yearly (365 days).  
- **Dynamic Calculations** – Updates instantly as you change amount/date.  
- **Installable PWA**  
  - Add to Home Screen on Android (Install button or Chrome menu).  
  - Add to Home Screen on iOS (Safari → Share → Add to Home Screen).  
- **Offline Support** – Works without internet after the first load (service worker caching).  

---

## 📊 Interest Calculation Logic

- **Monthly (30 days)**:  
  `Monthly Interest = Principal × 1.25%`  

- **Daily**:  
  `Daily Interest = Monthly Interest ÷ 30`  

- **Yearly (365 days)**:  
  `Yearly Interest = Daily Interest × 365`  

- For elapsed **N days**:  
  - Daily-based: `Daily Interest × N`  
  - Monthly equivalent: `Monthly Interest × (N ÷ 30)`  
  - Yearly equivalent: `Yearly Interest × (N ÷ 365)`  

---

## 🚀 Installation & Usage

### Run locally
1. Download this repo or ZIP.  
2. Open `index.html` in any browser.  
3. Start using – no server needed.

### Deploy on GitHub Pages
1. Push the repo to GitHub.  
2. Go to **Settings → Pages → Build and deployment → Deploy from a branch**.  
3. Select `main` (or default branch) and folder `/ (root)`.  
4. Save and open the GitHub Pages URL.  

### Install as App (PWA)
- **Android (Chrome):**  
  - Tap the blue **Install App** button OR  
  - Open Chrome menu **⋮ → Add to Home screen**.  
- **iOS (Safari):**  
  - Tap **Share → Add to Home Screen**.  
  - iOS doesn’t show install prompts, so follow the instructions shown in the app.  

---

## 🖼️ Screenshots

_(Add screenshots after you host it on GitHub Pages.)_

---

## 🛠️ Tech Stack

- **HTML5 + CSS + Bootstrap 5** – Responsive, mobile-first UI.  
- **JavaScript** – Dynamic calculations and validation.  
- **PWA** – `manifest.webmanifest` + `service worker (sw.js)` for offline support.  
- **Icons** – Multiple sizes (192, 512, 1024) with maskable support for Android/iOS.  

---

## 👤 Credits

Developed by **Meenakshi Finance** to simplify interest calculations for everyday use in Tamil Nadu.
