# Meenakshi Finance — Mobile PWA (Tamil)

A mobile-first **interest calculator + QR receipt generator** built for Tamil users. Designed to run easily on phones and installable as a **Progressive Web App (PWA)**.

## ✨ Features
- **Tamil UI** with large, touch-friendly controls
- **Primary: Interest calculator** at a fixed **1.25% monthly** rate
- **Porul (பொருள்) section** — optional, collapsible:
  - Receipt ID, Customer Name, Product details
- **Duration (காலம்)** shows **exact Years/Months/Days** (e.g., `3 வருடம் 2 மாதம் 2 நாள்`) and total days
- **Automatic summaries** for daily, monthly (30-day), yearly (365-day) interest
- **QR receipt** generation (text-encoded)
- **Share / WhatsApp**: pre-fills a message so users can send via WhatsApp
- **Copy to clipboard** for the receipt text
- **Installable PWA** with offline cache via Service Worker

## 📦 Files
```
.
├─ index.html
├─ manifest.webmanifest
├─ sw.js
└─ icons/
   ├─ icon-192.png
   ├─ icon-512.png
   └─ maskable-512.png
```

## 🚀 Deploy on GitHub Pages
1. Create a new repository (or use an existing one), e.g. `meenakshi-finance-pwa`.
2. Copy all files from this folder to your repository root.
3. Commit & push.
4. Enable **GitHub Pages** (Settings → Pages → Source: `main` → `/root`).
5. Visit the published URL (e.g. `https://<your-username>.github.io/meenakshi-finance-pwa/`).
6. On mobile, use **“Add to Home Screen”** to install.

> Tip: If you host the app in a subfolder, keep paths as relative (`./…`) exactly as provided.

## 🧮 Calculation details
- **Monthly rate:** 1.25% of principal (P)
- **Daily rate:** `monthly / 30`
- **Yearly rate:** `daily * 365`
- **Total days:** difference between start date and today (UTC midnight basis)
- **Duration field:** shows exact **Y/M/D breakdown** using 365-day year & 30-day month for readability.

## 🔐 Privacy
- No data is sent to a server; all calculations run in the browser.
- WhatsApp share opens the app with a **pre-filled message**; user decides whom to send.

## 🛠 Local development
Just open `index.html` in a modern browser. For full PWA behavior (service worker), serve via any static server or use GitHub Pages.

---

© 2025 Meenakshi Finance — Built for Tamil users.
