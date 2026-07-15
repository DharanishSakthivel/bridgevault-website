# BridgeVault Technology — Website Walkthrough & Deployment Guide

> **Version:** 1.1.0 · **Build:** 2026-07-15  
> **Status:** ✅ Production Ready — Dark/Light Theme Switching, Zero-dependency, GitHub Pages compatible

---

## 1. Project Overview

**BridgeVault Technology** is a complete, production-grade single-page enterprise web portal built with:
- **Pure HTML5** — Semantic, accessible, SEO-optimised heading structure.
- **Vanilla CSS** — CSS variables (custom properties) driving dual light/dark themes, CSS Grid, Flexbox, and micro-animations.
- **Vanilla JS** — High-performance background particle engine, scroll triggers, stat countup controllers, hamburger drawer menu, and LocalStorage-persisted theme switcher (prevents Flash of Unstyled Content).
- **Zero runtime dependencies** — Zero frameworks, zero compilers, ready for immediate static site deployment.

---

## 2. Directory Structure

```text
bridgevault_website/
├── index.html                  ← Master production SPA file (HTML, CSS, JS)
├── walkthrough.md              ← Deployment walkthrough and checklist
└── assets/
    ├── logo_minimal.svg        ← Vector corporate logo lockup with horizontal divider line
    └── social/
        └── linkedin_hero.svg   ← LinkedIn banner 1584×396 (SVG)
```

---

## 3. Local Preview & Testing

### Option A: Direct File Open (Fastest)
Double-click `index.html` in your file browser or drag it into any modern web browser.

### Option B: Using Python's built-in server
```bash
cd C:\Users\hp\.gemini\antigravity\scratch\bridgevault_website
python -m http.server 8080
# Then open: http://localhost:8080
```

---

## 4. GitHub Pages Deployment (Free Hosting)

### Step 1 — Create a GitHub Repository
1. Go to [github.com/new](https://github.com/new).
2. Repository name: `bridgevault-website`.
3. Set to **Public**.
4. Click **Create repository**.

### Step 2 — Push Files
```bash
cd C:\Users\hp\.gemini\antigravity\scratch\bridgevault_website
git init
git add .
git commit -m "feat: BridgeVault Technology — production light/dark theme release"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/bridgevault-website.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. Go to your repository on GitHub.
2. Click **Settings** → **Pages** (left sidebar).
3. Under **Source**: Select `Deploy from a branch`.
4. Branch: `main`, Folder: `/ (root)`.
5. Click **Save**.

---

## 5. Master Verification Checklist

### 5.1 — Visual Themes (Dark / Light Options)
- [ ] Theme toggler button appears in the desktop navigation bar (next to "Connect With Us") and mobile drawer list.
- [ ] Clicking toggle transitions variables immediately:
  - **Dark mode (Default)**: Background is `#030712`, card bases are `#060D1E` / `#0B1729`, text is `#FFFFFF`.
  - **Light mode**: Background transitions to Slate `#F8FAFC`, cards to pure white `#FFFFFF` with Slate `#E2E8F0` details, text becomes deep Slate `#0F172A`.
- [ ] The SVG wordmark text "Vault" changes dynamically (white in dark mode, slate in light mode).
- [ ] Selecting light/dark mode and refreshing preserves the selection via LocalStorage (zero flash of default mode on reload).

### 5.2 — Typography & Brand Assets
- [ ] Unified SVG logo shows the arch gate mark on the left, a thin vertical divider, and the "Bridge Vault" wordmark.
- [ ] The horizontal amber divider line is aligned **perfectly in between** "BridgeVault" and the tracked sub-label "TECHNOLOGY".
- [ ] Serving leaders horizontal strip lists **Pharma** and **Data Engineering** as core industries.

### 5.3 — Balanced Service Metrics (Credibility)
- [ ] Hero stats row and statistics section display balanced numbers representing all three core domains:
  - **Digital Engineering**: `120+ Production Systems Launched`
  - **Talent/Recruitment**: `98% Talent Retention Rate`
  - **Operations/BPO**: `99.8% SLA Operations Accuracy`
  - **Guarantees**: `90-Day Talent Placement Guarantee`
- [ ] The "Why BridgeVault" grid displays 6 balanced service cards.
- [ ] Engaging and realistic placements metrics are set: *`1,500+ successful engagements`* replaces legacy `10,000+` plannings.

### 5.4 — Scanning Methodology Visual
- [ ] Process section displays the reverted corporate scanning arch gate visual.
- [ ] Built-in scanning cyan laser line sweeps up and down the arch using a self-contained CSS keyframe animation.
- [ ] Glowing node endpoints and structural grid lines render smoothly.

### 5.5 — Social Links Loop
- [ ] Footer social menu loops 5 complete profiles:
  - **Instagram**: Link pointing to `https://instagram.com/bridgevault`
  - **LinkedIn**: Link pointing to `https://linkedin.com/company/bridgevault`
  - **Twitter/X**: Link pointing to `https://twitter.com/bridgevault`
  - **Email**: Link pointing to `mailto:dharanishsakthivel@outlook.com`
  - **WhatsApp**: Link pointing to `https://wa.me/918190044198`

---

*BridgeVault Technology LLP · Bridging Talent. Vaulting Innovation.*  
*Workspace: `C:\Users\hp\.gemini\antigravity\scratch\bridgevault_website\`*
