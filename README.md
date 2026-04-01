# coffeecoder.co.uk — Portfolio Site

Personal portfolio site for [Alexander Shannon](https://www.coffeecoder.co.uk) — Founding Engineer & Tech Lead.

Built with plain HTML, CSS and JavaScript. Hosted on Azure Static Web Apps with automatic CI/CD via GitHub Actions.

## 🌐 Live Site

- **Primary:** https://www.coffeecoder.co.uk
- **Default (Azure):** https://mango-sand-0a0494803.4.azurestaticapps.net

---

## 🏗️ Stack

| Layer | Technology |
|---|---|
| Site | Plain HTML / CSS / JS (no build tools) |
| Hosting | Azure Static Web Apps (Free tier) |
| DNS | Azure DNS (`coffeecoder.co.uk`) |
| CI/CD | GitHub Actions — auto-deploys on push to `main` |

---

## 🚀 Running Locally

No build step required — it's plain HTML/CSS/JS.

### Option 1 — Open directly in browser

```bash
open index.html
```

> Note: Some browsers may restrict local file access for fonts/assets. Use Option 2 for a better local experience.

### Option 2 — Local dev server (recommended)

Using [VS Code Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer):
1. Open the repo folder in VS Code
2. Right-click `index.html` → **Open with Live Server**

Or using Python's built-in server:

```bash
# Python 3
python3 -m http.server 8080
```

Then visit: http://localhost:8080

Or using Node's `serve`:

```bash
npx serve .
```

Then visit: http://localhost:3000

---

## 📁 Structure

```
├── index.html        # Main site (single page)
├── styles.css        # All styles
├── .github/
│   └── workflows/
│       └── azure-static-web-apps-*.yml   # CI/CD deploy workflow
└── README.md
```

---

## ✏️ Making Changes

1. Edit `index.html` and/or `styles.css`
2. Commit and push to `main`
3. GitHub Actions will automatically deploy to Azure Static Web Apps (~2 mins)

---

## ☁️ Infrastructure

- **Resource group:** `coffee-coder`
- **Static Web App:** `coffeecoder-portfolio`
- **DNS Zone:** `coffeecoder.co.uk`
- **Subscription:** Pay-As-You-Go

Monthly cost: ~£0.50/month (Azure DNS zone only — everything else is free tier).
