# 🚀 Impel Laboratories DBMS — Deployment Guide

## How to Deploy (Step-by-Step)

---

### STEP 1 — Install Node.js (if not installed)
1. Go to: https://nodejs.org
2. Download the **LTS version** (recommended)
3. Install it on your computer
4. Verify: open Terminal/Command Prompt → type `node -v` → should show a version number

---

### STEP 2 — Create a GitHub Account (if you don't have one)
1. Go to: https://github.com
2. Click **Sign up** → enter your email, create password
3. Verify your email

---

### STEP 3 — Create a New GitHub Repository
1. Log in to GitHub
2. Click the **+** button (top-right) → **New repository**
3. Repository name: `impel-labs-dbms`
4. Set it to **Public** (required for free Vercel hosting)
5. Click **Create repository**
6. Copy the repository URL shown (e.g. `https://github.com/yourusername/impel-labs-dbms.git`)

---

### STEP 4 — Upload Your Project to GitHub
Open Terminal / Command Prompt, then run these commands one by one:

```bash
# Navigate into this folder (change the path to where you extracted the ZIP)
cd /path/to/impel-labs

# Initialize git
git init

# Add all files
git add .

# Make your first commit
git commit -m "Initial commit: Impel Labs DBMS"

# Connect to your GitHub repo (paste YOUR repo URL here)
git remote add origin https://github.com/yourusername/impel-labs-dbms.git

# Push to GitHub
git branch -M main
git push -u origin main
```

✅ Your code is now on GitHub!

---

### STEP 5 — Deploy on Vercel (Free Hosting)
1. Go to: https://vercel.com
2. Click **Sign up** → choose **Continue with GitHub** → authorize
3. Click **Add New Project**
4. Find `impel-labs-dbms` in the list → click **Import**
5. Framework Preset: **Vite** (auto-detected)
6. Click **Deploy**
7. Wait 1–2 minutes ⏳

---

### STEP 6 — Your App is Live! 🎉
After deployment, Vercel gives you a URL like:
```
https://impel-labs-dbms.vercel.app
```
This URL opens in any browser worldwide — desktop or mobile.

---

### STEP 7 — Get a Custom Domain (Optional)
You can connect your own domain like `dbms.impellaboratories.com`:
1. In Vercel dashboard → your project → **Settings** → **Domains**
2. Add your domain and follow the DNS instructions

---

## Local Development (Run on Your Computer)

```bash
# Install dependencies (only first time)
npm install

# Start development server
npm run dev

# Open in browser
http://localhost:5173
```

---

## Project Structure

```
impel-labs/
├── public/
│   └── favicon.svg          ← App icon
├── src/
│   ├── main.jsx             ← React entry point
│   └── App.jsx              ← All modules (Dashboard, Sales, etc.)
├── index.html               ← HTML shell
├── package.json             ← Dependencies
├── vite.config.js           ← Build config
├── vercel.json              ← Deployment config
└── .gitignore               ← Files to ignore
```

---

## Modules Included

| Module             | Features                                      |
|--------------------|-----------------------------------------------|
| Dashboard          | KPIs, charts, activity feed, stock alerts     |
| Customer Mgmt      | Add/edit/delete, balance tracking             |
| Product Mgmt       | Pricing, stock, category management           |
| Sales & Invoices   | Transactions, dispatch, status tracking       |
| Tele-Sales         | Call queue, follow-ups, conversion tracking   |
| Production         | Batch logging, materials tracking             |
| Inventory          | Stock levels, low-stock alerts, reorder points|
| Audit Trail        | Full activity log with filters                |
| User Management    | Role-based access, 2FA, permissions           |

---

## Next Steps (Future Enhancements)

1. **Real Database** → Connect Supabase (free PostgreSQL)
2. **Authentication** → Add login with Supabase Auth or Firebase
3. **File Uploads** → Store invoices/CNs in Supabase Storage
4. **Offline Support** → Add PWA manifest + service worker
5. **Export to Excel** → Integrate SheetJS library
6. **Email Reports** → Use EmailJS or Supabase Edge Functions
7. **2FA** → Integrate TOTP via Supabase Auth

---

Built for **Impel Laboratories — Unani Medicine Manufacturer**
