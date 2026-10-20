# 💎 Plus UI — Glassmorphism Edition (PWA & 100% Owned)

[![Blogger Theme](https://img.shields.io/badge/Blogger-Theme%20v3.7.0-ff5722?style=for-the-badge&logo=blogger&logoColor=white)](https://blogger.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![PWA Ready](https://img.shields.io/badge/PWA-100%25%20Ready-00c853?style=for-the-badge&logo=pwa&logoColor=white)](manifest.json)
[![UI: Glassmorphism](https://img.shields.io/badge/Design-Glassmorphism%20v2-6366f1?style=for-the-badge)](https://github.com)

A modern, ultra-fast, and fully customizable **Glassmorphism Blogger Template** with **Progressive Web App (PWA)** capabilities, offline caching, and **100% clean, independent ownership**.

---

## ✨ Features

### 🪟 1. Pure Glassmorphism Design System
- **Dynamic Ambient Canvas**: Animated ambient radial light mesh providing realistic optical frosted glass effects.
- **Frosted Translucent Cards**: Cards and widgets use modern `backdrop-filter: blur(16px)` with delicate light borders (`rgba(255, 255, 255, 0.6)`).
- **Glassmorphic Sticky Header & Floating Navigation**: Seamless blur effect when scrolling over articles and images.
- **Glass Hover Elevate**: Smooth 3D-like hover lift with ambient colorful glowing drop shadows.
- **Dual Light / Dark Mode Synergy**: 
  - *Light Mode*: Frosted crystalline white surface with indigo/cyan ambient reflections.
  - *Dark Mode*: Deep slate translucent glass (`rgba(15, 23, 42, 0.74)`) with neon aura lights.

### 📱 2. Premium Progressive Web App (PWA) Engine
- **Ultra-Premium Glass Install Prompt**: Replaces typical crude alert banners with an elegant frosted glass bottom card featuring micro-animations, feature tags, and quick-action buttons.
- **Smart Engagement Logic**: Appears gracefully after user interaction (6 seconds) without aggressive spamming; respects user dismissal for 7 days.
- **Service Worker (`sw.js`)**:
  - Offline fallback caching for instant loads.
  - Network-first caching strategy for fresh content with cache fallback.
- **Full Web App Manifest (`manifest.json`)**: Configured with shortcuts, standalone display, maskable icons, and theme color harmonization.

### 🛡️ 3. 100% Clean Ownership (No Backdoors / Traps)
- **Zero Obfuscated Trackers**: All third-party redirect traps and hidden SEO injections have been completely removed.
- **Customizable Footer**: Freedom to edit copyright credits via Blogger Layout without forced redirects.
- **Self-Contained & Independent**: No dependency on external proprietary licensing servers.

---

## 📁 Repository Structure

```text
├── PLUS-UI.xml               # Primary Glassmorphism Blogger XML Template
├── manifest.json             # PWA Web App Manifest
├── sw.js                     # PWA Service Worker (Offline caching engine)
├── app/
│   └── manifest.webmanifest # Secondary webmanifest route
├── LICENSE                   # Open-Source MIT License
└── README.md                 # Documentation
```

---

## 🚀 Installation Guide (Blogger / Blogspot)

1. **Download Theme**: Clone or download `PLUS-UI.xml` from this repository.
2. **Access Blogger**:
   - Go to [Blogger Dashboard](https://www.blogger.com) > **Theme**.
   - Click the drop-down menu next to **Customize** > Select **Restore**.
   - Upload `PLUS-UI.xml`.
3. **Turn off Mobile Theme**:
   - Click drop-down next to **Customize** > **Mobile Settings** > Select **Desktop** > Save.
4. **PWA Setup**:
   - The theme dynamically manages the PWA manifest and service worker.
   - For custom icons and titles, update the **Progressive Web App** LinkList widget inside **Blogger Layout**.

---

## 🎨 Glassmorphism CSS Customization

You can fine-tune the glass aesthetics directly within the template `:root` stylesheet:

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

## 📄 License

This theme is released under the **[MIT License](LICENSE)**. You are 100% free to modify, customize, rebrand, and deploy it for personal and commercial projects.
