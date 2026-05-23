# Odoo Note Cleaner

AI-powered tool to clean and structure Odoo CRM notes exported as CSV.

## How to Deploy (Free - 10 minutes)

### Step 1 — Upload to GitHub
1. Go to https://github.com and sign up / log in
2. Click **New Repository** (green button)
3. Name it: `odoo-note-cleaner`
4. Click **Create repository**
5. Click **uploading an existing file**
6. Upload ALL files from this folder (index.html, vercel.json, README.md)
7. Click **Commit changes**

### Step 2 — Deploy on Vercel
1. Go to https://vercel.com and sign up with your GitHub account
2. Click **Add New Project**
3. Select your `odoo-note-cleaner` repository
4. Click **Deploy** (no settings needed)
5. Wait ~1 minute — Vercel gives you a live link!

### Step 3 — Share the link
Your app will be live at: `https://odoo-note-cleaner.vercel.app`
Share this with anyone — they just need their own Anthropic API key.

## How to Get Anthropic API Key (Free)
1. Go to https://console.anthropic.com
2. Sign up for free
3. Go to **API Keys** section
4. Click **Create Key**
5. Copy and paste it into the app

## How the App Works
1. User enters their Anthropic API key (stored only in their browser)
2. User uploads CSV exported from Odoo
3. Claude AI reads each note and extracts:
   - Requirement (product/service needed)
   - Status (Purchase Done / Pending / Follow-up / Open)
   - Vendor name
   - Timeline
   - Follow-up status
   - Clean English summary
4. User downloads the structured CSV

## Files
- `public/index.html` — The complete web app (single file)
- `vercel.json` — Vercel deployment config
