# Baseline Abode Initiative

The **Baseline Abode Initiative (BAI)** is a conceptual and technical framework for modeling housing entitlement based on lifetime productive contribution using Energy Credits.

This repository contains:

- `index.html` — BAU calculator (household + national scenario modeling)
- `manifesto.html` — philosophical and structural foundation of the initiative
- `manifest.json` — PWA configuration
- `service-worker.js` — offline capability
- `styles.css` — styling
- `/icons` — PWA and maskable icons

---

## 🧠 Concept Overview

The BAU model introduces a simple constraint:

> **A system cannot yield more than is contributed into it.**

Energy Credits represent a normalized unit of productive value:
- May be benchmarked to real energy (e.g., kWh)
- May represent broader economic and infrastructure output
- Are used to determine housing capacity over time

---

## 📱 Progressive Web App (PWA)

This application is installable and works offline.

### Requirements
- HTTPS hosting (GitHub Pages supported)
- Modern browser (Chrome, Edge, Safari)

### Features
- Install to home screen
- Offline access via service worker
- Responsive across desktop and mobile

---

## 🚀 Running Locally

Use a local server (service workers require it):

### Option 1: Python
```bash
python -m http.server 8080