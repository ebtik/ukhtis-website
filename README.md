# UKHTIS Website Setup Guide

## Your Folder Structure
```
ukhtis-site/
├── index.html          ← Your main website
├── netlify.toml        ← Netlify config
├── admin/
│   ├── index.html      ← CMS login page
│   └── config.yml      ← CMS settings (what's editable)
├── _data/
│   ├── settings.json   ← Site-wide text settings
│   ├── abayas/         ← Your products go here
│   ├── services/       ← Your services
│   ├── coming_soon/    ← Coming soon items
│   └── announcements/  ← Top bar messages
└── images/             ← Upload your photos here
```

---

## Step-by-Step Setup

### 1. Create GitHub Account
Go to github.com → Sign up (free)

### 2. Create New Repository
- Click + → New repository
- Name: ukhtis-website
- Set to Public
- Click Create repository

### 3. Upload All Files
- Click "uploading an existing file"
- Upload ALL files and folders from this zip
- Keep the folder structure exactly as is
- Click Commit changes

### 4. Deploy on Netlify
- Go to netlify.com → Sign up with GitHub
- Click "Add new site" → "Import from Git"
- Choose GitHub → select ukhtis-website
- Click Deploy Site
- Wait ~1 minute → your site is live!

### 5. Enable Identity (for CMS login)
- In Netlify → Site Settings → Identity
- Click "Enable Identity"
- Under Registration → change to "Invite only"
- Under Services → Git Gateway → Enable Git Gateway
- Go to Identity tab → Invite users → enter YOUR email
- Check your email → accept the invite → set a password

### 6. Connect ukhtis.co
- In Netlify → Domain Management → Add custom domain
- Type: ukhtis.co → Confirm
- Copy the 2 nameserver addresses Netlify gives you
- Go to Spaceship.com → your domain → Nameservers → Custom
- Paste Netlify's nameservers → Save
- Wait 24 hours → done ✅

---

## How to Edit Your Website

Go to: **ukhtis.co/admin** (or yoursite.netlify.app/admin)
Log in with your email/password

### Add a Product (Abaya)
1. Click "🧕 Abayas" in the left menu
2. Click "New Abaya"
3. Fill in: Name, Label, Description, Price, upload Photo
4. Click Publish → appears on website in ~30 seconds

### Edit Site Text
1. Click "⚙️ Site Settings"
2. Change hero text, tagline, about story, WhatsApp number
3. Click Save

### Add Announcement Bar
1. Click "📢 Announcements"
2. New Announcement → type your message → toggle Active ON
3. Save → appears at top of website

---

## Your CMS Dashboard URL
After setup: ukhtis.co/admin
