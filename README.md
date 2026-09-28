# 🏨 Thanima Farm Life / Resort - Daily Operations & Security Management

A modern, highly responsive, and mobile-optimized Daily Operations and Security Reporting System with seamless WhatsApp connectivity.

Built with vanilla HTML, modern CSS, and JavaScript. Zero external dependencies, lightning fast, works completely offline, and ready for deployment on GitHub Pages.

---

## ✨ Features & Improvements

### 📱 1. Fully Responsive & Mobile-First Design
- **Touch-Friendly Controls**: Minimum 48px tap targets with numeric stepper (`+`/`−`) buttons for one-handed operation on mobile devices.
- **Dynamic Layout**: Smoothly adapts from small mobile screens (320px+) to tablets and ultra-wide desktop monitors.
- **Safe Area Inset Support**: Full viewport coverage with support for modern smartphone notches and navigation bars (`viewport-fit=cover`).
- **Dark / Light Theme**: Instant switch between daytime high-contrast mode and eye-friendly dark mode for nighttime security duty.

### 💬 2. WhatsApp Integration & Dispatch
- **Direct Chat & Web Links**: Send formatted daily reports directly via WhatsApp mobile app, desktop app, or WhatsApp Web (`web.whatsapp.com`).
- **Country Code Selector**: Pre-configured international dial codes (+91 India, +971 UAE, +966 KSA, +974 QA, +44 UK, +1 US, etc.).
- **Frequent Contact Book**: Save key recipient phone numbers (e.g. "Operations Manager", "Front Office Lead", "Security Lead") directly in the browser for 1-click selection.
- **Native Web Share**: Uses the device's native sharing sheet (`navigator.share`) to dispatch to WhatsApp groups or any messaging app.
- **1-Click Copy**: Copy formatted WhatsApp text to clipboard with instant confirmation toast.
- **Realistic WhatsApp Chat Simulation**: Live preview bubble showing exactly how formatting (bolding, lists, timestamps) will appear inside WhatsApp.

### 🛡️ 3. Bug Fixes & Reliability Enhancements
- **Timezone Date Bug Fixed**: Resolved UTC midnight offset issue in standard JavaScript `new Date()` that previously displayed incorrect previous-day dates in certain timezones.
- **Live Reactive Updates**: Dynamic lists (food items, materials inward) now immediately update the WhatsApp preview when added, edited, or deleted.
- **Smart Text Parsing**:
  - Automatically splits entries like `"Cookies 36.5 kg"` into Name: `Cookies`, Quantity: `36.5`, Unit: `kg`.
  - Automatically splits entries like `"Omelet 2"` into Name: `Omelet`, Quantity: `2`.
- **Auto-Save Drafts**: Automatically stores form inputs in browser `localStorage`. If the browser tab is accidentally refreshed or closed, all typed data is preserved.
- **Integrity Validation Badges**: Real-time counter verifying whether subcategories (e.g. Day out + Stay + Evening) match total counts.
- **Negative Value Prevention**: Guard rails enforcing non-negative numeric inputs.

---

## 🚀 How to Run Locally

No server or npm installation needed! You can open the file directly in any modern browser:

1. Double-click `index.html` (or `nimisha.html`) in File Explorer.
2. Or serve locally with Python:
   ```bash
   python -m http.server 8000
   ```
   and navigate to `http://localhost:8000` in your web browser.

---

## 🌐 Deploy to GitHub Pages

1. Go to your repository settings on GitHub.
2. Navigate to **Pages** in the left sidebar.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Choose the `main` branch and `/ (root)` folder, then click **Save**.
5. Your daily report app will be live on `https://<username>.github.io/Security-report-management/`!

---

## 📄 License
MIT License
