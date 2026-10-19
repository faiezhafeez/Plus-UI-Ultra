# 📘 Plus UI Ultra — Complete Theme Setup & Customization Guide

Welcome to the official setup documentation for **Plus UI Ultra (Glassmorphism & PWA Edition)** developed and maintained by **Faiez Hafeez**.

---

## 📑 Table of Contents
1. [Prerequisites](#1-prerequisites)
2. [Step-by-Step Installation on Blogger](#2-step-by-step-installation-on-blogger)
3. [Crucial: Desktop Mode Setting for Mobile](#3-crucial-desktop-mode-setting-for-mobile)
4. [Setting Up Progressive Web App (PWA)](#4-setting-up-progressive-web-app-pwa)
5. [Configuring Navigation Menu & Search](#5-configuring-navigation-menu--search)
6. [Dark Mode & Theme Scheme Customization](#6-dark-mode--theme-scheme-customization)
7. [Glassmorphism Visual Controls & CSS Tweaks](#7-glassmorphism-visual-controls--css-tweaks)
8. [Configuring Footer Copyright](#8-configuring-footer-copyright)
9. [Troubleshooting & FAQs](#9-troubleshooting--faqs)

---

## 1. Prerequisites
- A Google account with access to [Blogger.com](https://www.blogger.com).
- Downloaded `PLUS-UI.xml` file from this repository.
- Recommended browser for testing PWA: Google Chrome, Microsoft Edge, or Safari on iOS.

---

## 2. Step-by-Step Installation on Blogger

1. Log in to your [Blogger Dashboard](https://www.blogger.com).
2. On the left navigation sidebar, click on **Theme**.
3. Next to the orange **CUSTOMIZE** button, click the downward arrow (**▼**).
4. Select **Backup** first to download your current theme as a safety measure.
5. Click the downward arrow (**▼**) again and select **Restore**.
6. Click **Upload** and browse to select `PLUS-UI.xml` from your computer.
7. Wait 5-10 seconds until Blogger displays *"Theme restored"*.

---

## 3. Crucial: Desktop Mode Setting for Mobile

> ⚠️ **IMPORTANT**: If this step is skipped, mobile visitors will see Blogger's old default mobile template instead of Plus UI Ultra's responsive Glassmorphic layout.

1. Go to **Theme** > click the downward arrow (**▼**) next to **Customize**.
2. Click **Mobile settings**.
3. Select **Desktop** (do *not* select Mobile default).
4. Click **Save**.

Now your blog will render the ultra-sleek, responsive Glassmorphism design across all smartphone screens, tablets, laptops, and desktop monitors.

---

## 4. Setting Up Progressive Web App (PWA)

Plus UI Ultra comes equipped with an ultra-premium frosted glass PWA install prompt and offline caching engine.

### How it works:
1. **Auto-Trigger**: Visitors browsing your website for more than 6 seconds will see a floating frosted glass install banner.
2. **Service Worker (`sw.js`)**: Automatically precaches core assets and provides offline fallback navigation.
3. **Customizing PWA Metadata via Blogger Layout**:
   - Go to **Layout** > scroll down to **Addon Widgets** section.
   - Locate the **Progressive Web App** (`LinkList`) widget.
   - You can configure:
     - `name`: Full title of your App.
     - `short_name`: Short title for app homescreen.
     - `description`: Subtitle or tag line.
     - `theme_color`: Primary browser header color (`#6366f1`).
     - `background_color`: Splash screen background (`#0b0f19`).
     - `icon`: Square PNG URL (minimum 192x192, recommended 512x512).

---

## 5. Configuring Navigation Menu & Search

### Navigation Menu Setup:
1. Go to **Layout** > **Header Menu / Main Menu** widget.
2. Add links using the following structure:
   - Normal link: `Home` -> `/`
   - Sub-menu item: `_Sub Item 1` (prefix with an underscore `_`)
   - Second-level sub-menu: `__Nested Item` (prefix with two underscores `__`)
   - Mega menu label: `Notes [mega]` (append `[mega]` to trigger rich mega post preview)

### Live Search Modal:
The search engine is built directly into the header. Clicking the magnifying glass icon opens the frosted glass search modal (`.sMdl`) with instant AJAX results as the user types.

---

## 6. Dark Mode & Theme Scheme Customization

Plus UI Ultra supports **Automatic System Preference**, **Light Mode**, and **Dark Mode** with view transitions.

### Default Mode Configuration:
In `PLUS-UI.xml` (or via Theme variables in Theme > Customize):
- `style.defaultMode`:
  - `1px` = Light mode default
  - `2px` = Dark mode default
  - `3px` = Follows visitor's OS system mode (Auto)

Visitors can toggle modes anytime using the moon/sun button on the header or floating dock.

---

## 7. Glassmorphism Visual Controls & CSS Tweaks

To customize the frosted blur strength, translucent background opacity, or accent colors, edit the CSS variables inside `<b:skin>` in `PLUS-UI.xml`:

```css
:root {
  /* Card Blur Strength */
  --glass-blur: blur(16px);          /* Standard card blur */
  --glass-blur-deep: blur(24px);     /* Modal & Header blur */

  /* Translucent Surface Colors */
  --glass-bg: rgba(255, 255, 255, 0.68);      /* Light mode card fill */
  --glass-border: rgba(255, 255, 255, 0.6);   /* Light mode rim light */
  
  /* Primary Accent & Glow */
  --glass-accent: #6366f1;                    /* Indigo vibrant accent */
  --glass-accent-glow: rgba(99, 102, 241, 0.28);
}

/* Dark Mode Adjustments */
.drK, [data-theme='dark'] {
  --glass-bg: rgba(15, 23, 42, 0.74);         /* Deep slate glass */
  --glass-border: rgba(255, 255, 255, 0.1);   /* Subtle neon edge */
  --glass-accent: #818cf8;
}
```

---

## 8. Configuring Footer Copyright

1. Go to **Layout** > scroll to **Footer** > find **Credit** widget (`HTML21`).
2. You can leave it empty to use the automatic dynamic copyright:
   ```html
   © 2026 Your Blog Name. Powered by Plus UI Ultra
   ```
3. Or write any custom HTML you want! There are zero forced redirects or obfuscated scripts.

---

## 9. Troubleshooting & FAQs

### Q1: The PWA banner does not appear when testing locally.
- **Answer**: PWA requires a valid `HTTPS` connection (or `localhost`). Ensure your Blogger blog has **HTTPS Redirect** turned ON in **Settings > HTTPS**. Also, if you already clicked "Later", the prompt sleeps for 7 days (clear `localStorage` in browser DevTools to test again).

### Q2: Blogger gives an error: *"Your template could not be parsed as it is not well-formed"*.
- **Answer**: Ensure you uploaded the exact unmodified `PLUS-UI.xml` file. Do not copy-paste code through rich text editors (like MS Word) which replace standard quotes with smart quotes.

### Q3: How do I change the App Icon?
- **Answer**: Upload your 512x512 PNG image to Blogger or GitHub, copy the URL, and update `manifest.json` and the `Progressive Web App` widget in Blogger Layout.

---

### 👨‍💻 Author & Support
- Repository: [github.com/faiezhafeez/Plus-UI-Ultra](https://github.com/faiezhafeez/Plus-UI-Ultra)
- Created & Maintained by: **Faiez Hafeez**
- License: **MIT License** (Free for personal and commercial use)
