# APEX DM Operator Site

## Files
- `index.html` — Client-facing landing page
- `apply.html` — Application form (powered by Formspree)
- `dashboard.html` — Internal operator portal (password-gated)

---

## Deploy to GitHub Pages (Free — 5 steps)

### Step 1 — Create a free GitHub account
Go to https://github.com and sign up if you don't have one.

### Step 2 — Create a new repository
- Click the + icon → "New repository"
- Name it: `apex-dm-operator` (or anything you want)
- Set it to **Public**
- Click "Create repository"

### Step 3 — Upload your files
- On the repo page, click "uploading an existing file"
- Drag and drop all 3 HTML files (index.html, apply.html, dashboard.html)
- Click "Commit changes"

### Step 4 — Enable GitHub Pages
- Go to Settings (top tab of the repo)
- Click "Pages" in the left sidebar
- Under "Source" → select "Deploy from a branch"
- Branch: `main` / Folder: `/ (root)`
- Click Save

### Step 5 — Your site is live
GitHub will give you a URL like:
`https://yourusername.github.io/apex-dm-operator/`

Takes about 60 seconds to go live.

---

## Activate the Application Form

1. Go to https://formspree.io — create a free account
2. Click "New Form" — name it "APEX Applications"
3. Copy your Form ID (looks like: `xrgpjwzb`)
4. Open `apply.html`
5. Find this line:
   `action="https://formspree.io/f/YOUR_FORM_ID"`
6. Replace `YOUR_FORM_ID` with your actual ID
7. Re-upload apply.html to GitHub

All applications will go straight to your email. Free tier = 50 submissions/month.

---

## Change the Dashboard Password

1. Open `dashboard.html`
2. Find this line near the top of the `<script>` section:
   `const ACCESS_CODE = 'apex2025';`
3. Change `apex2025` to whatever you want
4. Re-upload dashboard.html to GitHub

---

## Custom Domain (Optional — Free)
If you want `yourdomain.com` instead of the GitHub URL:
- Buy a domain from Namecheap or Cloudflare (~$10/year)
- In GitHub Pages settings → add your custom domain
- Update your DNS records (GitHub gives you exact instructions)

---

## What the Dashboard Does
- **Overview tab**: Live KPI tracker (prospects, openers, convos, booked, show rate) with color coding against targets
- **Pipeline tab**: Full CRM — add prospects, track EAACO stage, momentum heat map, person type, notes
- **Daily Ops tab**: 90-minute mindframe checklist + pre-send Human Reasoning Stack checklist
- **Frameworks tab**: All 37 APEX frameworks as a quick-reference card deck
- **Notes tab**: Scratch pad for debriefs, KGA outputs, gap audits — auto-saves to browser

Everything saves locally in the browser (no server needed).
