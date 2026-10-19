# 💎 Plus UI Ultra — Glassmorphism & PWA Edition

[![GitHub Repo](https://img.shields.io/badge/GitHub-faiezhafeez%2FPlus--UI--Ultra-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/faiezhafeez/Plus-UI-Ultra)
[![Blogger Theme](https://img.shields.io/badge/Blogger-Theme%20v4.0.0-ff5722?style=for-the-badge&logo=blogger&logoColor=white)](https://blogger.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![PWA Ready](https://img.shields.io/badge/PWA-100%25%20Ready-00c853?style=for-the-badge&logo=pwa&logoColor=white)](manifest.json)
[![Design: Glassmorphism](https://img.shields.io/badge/Design-Glassmorphism%20v2-6366f1?style=for-the-badge)](https://github.com/faiezhafeez/Plus-UI-Ultra)

A modern, ultra-fast, and fully customizable **Glassmorphism Blogger Template** with **Progressive Web App (PWA)** capabilities, offline caching, and **100% clean, independent ownership** by **Faiez Hafeez**.

---

## 🌟 Highlights & Key Features

* **💎 Pure Glassmorphism Aesthetic**: Dynamic ambient radial light mesh, frosted acrylic cards with `backdrop-filter: blur(16px)`, translucent borders, and soft glowing elevation shadows.
* **📱 Ultra-Premium PWA Engine**: Floating frosted glass install prompt, offline service worker (`sw.js`), full web app manifest, maskable icons, and app shortcuts.
* **🛡️ 100% Complete Ownership**: Zero encrypted code, zero third-party copyright locks, zero backdoor redirects. Fully owned and MIT licensed.
* **⚡ Blazing Fast Performance**: Fully optimized assets, lazy loading (`lazysizes`), modern CSS variables, responsive across all screen sizes.
* **🌓 Dual Mode Synergy**: Flawless light and dark mode with smooth CSS view transitions.

---

## 📁 Repository Overview

```text
E:\Plus ui\
├── PLUS-UI.xml               # Complete Glassmorphism Blogger XML Theme File
├── SETUP_GUIDE.md            # Comprehensive Step-by-Step Setup & Customization Guide
├── manifest.json             # PWA Web App Manifest
├── sw.js                     # High-Performance Offline Caching Service Worker
├── app/
│   └── manifest.webmanifest # Secondary webmanifest route
├── .gitignore                # Git exclusions
├── LICENSE                   # Open-Source MIT License
└── README.md                 # Project Overview & Quick Start
```

---

## 🚀 Quick Setup Guide

For detailed, step-by-step instructions, read the **[Full Setup Guide (SETUP_GUIDE.md)](SETUP_GUIDE.md)**.

1. **Download Theme**: Clone or download [`PLUS-UI.xml`](PLUS-UI.xml) from this repository:
   ```bash
   git clone https://github.com/faiezhafeez/Plus-UI-Ultra.git
   ```
2. **Upload to Blogger**:
   - Go to **Blogger Dashboard** > **Theme**.
   - Click the drop-down menu next to **Customize** > Select **Restore**.
   - Upload `PLUS-UI.xml`.
3. **Crucial Mobile Setting**:
   - Next to **Customize**, click the arrow (**▼**) > **Mobile Settings** > Select **Desktop** > Save.
4. **PWA Activation**:
   - Automatic! The theme registers the Service Worker and presents a sleek frosted glass install banner after 6 seconds of engagement.

---

## 🛠️ Customizing Glassmorphism Colors

Fine-tune blur and translucent surface opacities directly in the template `:root` stylesheet:

```css
:root {
  --glass-bg: rgba(255, 255, 255, 0.68);         /* Frosted card fill */
  --glass-border: rgba(255, 255, 255, 0.6);        /* Card border rim */
  --glass-blur: blur(16px);                        /* Blur intensity */
  --glass-accent: #6366f1;                         /* Accent color */
  --glass-accent-glow: rgba(99, 102, 241, 0.28);   /* Glow shadow */
}
```

---

## 👨‍💻 Author & Contributions

* **Author**: [Faiez Hafeez](https://github.com/faiezhafeez)
* **Repository**: [github.com/faiezhafeez/Plus-UI-Ultra](https://github.com/faiezhafeez/Plus-UI-Ultra)
* **Contributions**: Issues, forks, and pull requests are welcomed!

---

## 📄 License

This project is licensed under the **[MIT License](LICENSE)** — free to use, customize, modify, and redistribute.
