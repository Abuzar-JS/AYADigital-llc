# AyaDigital LLC — Studio Hub & Store Compliance Portal

Official static website repository for **AyaDigital LLC**, an independent mobile app development studio.

This website serves as the central hub for Google Play Store and Apple App Store compliance, hosting the **Privacy Policy**, **Terms of Service**, and **Account Deletion** instructions for all published mobile applications, starting with **Hashyi (حاشي)** (`com.hashyi.app`).

---

## ⚡ Architecture & Design Principles

1. **Ultra-Lightweight & Zero Overhead:**
   - Pure static HTML5 and modern vanilla CSS (`styles.css`).
   - Zero JavaScript frameworks, zero external CDNs, zero analytics/tracking scripts.
   - Loads instantly (< 100ms) with a 100/100 Google Lighthouse score.
2. **Mobile-First & Responsive:**
   - Clean, modern typography using native system fonts.
   - Studio color scheme: deep slate, tech indigo, and warm sand/oasis accents.
   - Native bilingual layout support: Arabic (`dir="rtl"`) and English (`dir="ltr"`).
3. **Store Compliance Ready:**
   - Apple App Store Review Guideline 5.1.1(v) compliant account deletion flow.
   - Google Play Data Safety declaration and in-app/web erasure links.
   - Support & compliance email prominently featured: `tradea12027@gmail.com`.

---

## 📁 Repository Directory Structure

```text
ayadigital/
├── .nojekyll                  # Bypasses Jekyll on GitHub Pages for clean static serving
├── .gitignore                 # Standard git exclusions
├── README.md                  # Studio documentation and deployment guide
├── index.html                 # Studio landing page listing all apps & policies
├── styles.css                 # Clean, shared vanilla CSS design system
├── assets/
│   ├── logo.svg               # Modern geometric AyaDigital LLC studio mark
│   └── hashyi-icon.png        # Official Hashyi 512x512 app icon
└── hashyi/
    ├── index.html             # Hashyi Privacy Policy (bilingual Arabic & English)
    ├── privacy.html           # Canonical alias for direct /hashyi/privacy store links
    ├── delete-account.html    # Apple Guideline 5.1.1(v) & Google Play compliant deletion instructions
    └── terms.html             # Hashyi Terms of Service (bilingual Arabic & English)
```

---

## 🚀 How to Deploy to GitHub Pages

### 1. Push to GitHub
```bash
cd /home/abx/abx/go/src/github.com/Abuzar-JS/ayadigital

# Add remote
git remote add origin git@github.com-abuzar:Abuzar-JS/AYADigital-llc.git

# Push main branch
git push -u origin main
```

### 2. Enable GitHub Pages
1. Go to your repository on GitHub: `https://github.com/Abuzar-JS/AYADigital-llc`.
2. Click **Settings** &rarr; **Pages** (under Code and automation).
3. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Select `main` and folder `/ (root)`.
   - Click **Save**.
4. GitHub Pages will build and deploy the site in ~30 seconds at:
   ```text
   https://Abuzar-JS.github.io/AYADigital-llc/
   ```

### 3. Custom Domain Setup (Optional)
If you wish to attach a custom domain (e.g. `ayadigital.com` or `compliance.hashyi.com`):
1. In the repository root, add a file named `CNAME` with your domain:
   ```text
   compliance.ayadigital.com
   ```
2. Configure your DNS provider with a CNAME pointing to `<your-username>.github.io`.

---

## 📋 App Store & Google Play Submission URLs

For app submission of **Hashyi** (`com.hashyi.app`):

| Store Field | URL Path (Relative to Site Base) |
| :--- | :--- |
| **Privacy Policy URL** | `/hashyi/index.html` (or `/hashyi/`) |
| **Terms of Service URL** | `/hashyi/terms.html` |
| **Account Deletion URL (Apple 5.1.1(v))** | `/hashyi/delete-account.html` |
| **Support / Marketing URL** | `/index.html` |
| **Official Compliance Email** | `tradea12027@gmail.com` |

For app submission of **spaceO (سبيس أو)** (`com.spaceo.app`):

| Store Field | Public Live URL Path |
| :--- | :--- |
| **Privacy Policy URL** | `/spaceo-privacy.html` (or `/spaceo/`) |
| **Account Deletion URL (Apple 5.1.1(v) & Play Safety)** | `/spaceo-delete-account.html` |
| **Support / Marketing URL** | `/index.html` (or `https://spaceo.space/`) |
| **Official Compliance Email** | `tradea12027@gmail.com` |

---

## ➕ How to Add Future Apps

To register a new mobile app in this studio hub:

1. Create a new folder matching the app slug (e.g. `myapp/`):
   ```bash
   mkdir myapp
   ```
2. Add the app's policy pages:
   - `myapp/index.html` (Privacy Policy)
   - `myapp/terms.html` (Terms of Service)
   - `myapp/delete-account.html` (Account Deletion)
3. Add a new `<article class="card card-app">` in the root `index.html` under the **Published Mobile Applications** section with the app's icon, bundle ID, description, and links.

---

## 🛡️ Studio Support & Compliance

- **Company / Studio Name:** AyaDigital LLC
- **Compliance & Support Desk:** `tradea12027@gmail.com`
- **Response SLA:** Inquiries and deletion requests handled within 48 business hours.

&copy; 2026 AyaDigital LLC. All rights reserved.
