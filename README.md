# 📱 Meenakshi Finance - வட்டி கணக்கிடும் பயன்பாடு

A **Tamil-first Progressive Web App (PWA)** to calculate loan/pawn (`அடகு`) interest dynamically.  
The app is designed to be **simple, mobile-friendly, and senior-citizen friendly**, with a fixed **1.25% monthly interest rate**.

---

## ✨ Features

- **Tamil UI** 🇮🇳 – All labels, hints, and error messages are in Tamil.  
- **Fixed Interest Rate** – Always **1.25% per month**, read-only.  
- **Dynamic Date Input**  
  - Enter `அடகு பிடிப்பு தேதி` in **DD-MM-YYYY** format (keyboard)  
  - Or pick from the **calendar**  
  - Validates date and disallows future dates.  
- **Auto “Today”** – Today’s date is auto-filled and locked.  
- **Auto Days Calculation** – Number of days auto-calculated between start date and today.  
- **Breakdowns in Days, Months, Years**  
  - Example: `45 days → 1 month 15 days`  
  - Shows results for **Daily**, **Monthly (30 days)**, and **Yearly (365 days)** interest.  
- **Dynamic Calculation** – Updates automatically as soon as user changes amount/date.  
- **Installable Mobile App (PWA)**  
  - Add to Home Screen  
  - Full-screen standalone mode  
  - Works **offline** (cached with Service Worker)  

---

## 📊 Interest Calculation Logic

- **Monthly (30 days)**:  
  `Monthly Interest = Principal × 1.25%`  

- **Daily**:  
  `Daily Interest = Monthly Interest ÷ 30`  

- **Yearly (365 days)**:  
  `Yearly Interest = Daily Interest × 365`  

- For elapsed **N days**:  
  - Daily-based total: `Daily Interest × N`  
  - Monthly equivalent: `Monthly Interest × (N ÷ 30)`  
  - Yearly equivalent: `Yearly Interest × (N ÷ 365)`  

---

## 🚀 Installation / Deployment

### Run locally
1. Download the repository or ZIP.
2. Open `index.html` in your browser.
3. That’s it – no server needed.

### Deploy on GitHub Pages
1. Push repo to GitHub.  
2. Go to **Settings → Pages → Deploy from branch** → select `main` and `/ (root)`.  
3. After a minute, your app will be live at:  
   `https://<username>.github.io/<repo-name>/`

### Install as PWA
- On **mobile browsers** (Chrome, Edge, Safari), click **Install App / Add to Home Screen**.  
- The app runs **offline** after first use.  

---

## 🖼️ Screenshots

_(Add screenshots of the app here once hosted on GitHub Pages.)_

---

## 🛠️ Tech Stack

- **HTML5 + CSS + Bootstrap 5** – UI & mobile responsiveness  
- **JavaScript** – Dynamic calculations & validations  
- **PWA** – `manifest.webmanifest` + `service worker (sw.js)` for offline caching  

---

## 👤 Credits

Developed by **Meenakshi Finance** team to simplify interest calculations for everyday use.  

---
