# 🚀 Deployment Guide - ProBite Website

## Step-by-Step: Push to GitHub & Deploy

### 1️⃣ Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+" icon** (top right) → **"New repository"**
3. Fill in:
   - **Repository name:** `probite-website` (or your preferred name)
   - **Description:** "Premium protein balls website - ProBite"
   - **Visibility:** Choose Public or Private
   - ⚠️ **DO NOT** check "Add a README" (we already have one)
4. Click **"Create repository"**

### 2️⃣ Push Your Code to GitHub

Copy and run these commands in Terminal (from the ProBites folder):

```bash
# Navigate to the project folder
cd "/Users/asif/cursor projects/Mj/ProBites"

# Add GitHub as remote (replace YOUR-USERNAME and REPO-NAME)
git remote add origin https://github.com/YOUR-USERNAME/probite-website.git

# Rename branch to main (if needed)
git branch -M main

# Push to GitHub
git push -u origin main
```

**Example:**
```bash
git remote add origin https://github.com/johndoe/probite-website.git
git branch -M main
git push -u origin main
```

### 3️⃣ Enable GitHub Pages (Make it Live!)

1. Go to your repository on GitHub
2. Click **"Settings"** (top menu)
3. Scroll down and click **"Pages"** (left sidebar)
4. Under **"Source"**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **"Save"**
6. Wait 1-2 minutes for deployment
7. Your live URL will appear at the top:
   ```
   Your site is live at https://YOUR-USERNAME.github.io/probite-website/
   ```

### 4️⃣ Share with Your Client

Once deployed, share this information:

**📧 Email Template:**

```
Subject: ProBite Website Preview - Ready for Review

Hi [Client Name],

Your ProBite website is ready for preview! 🎉

🌐 Live Preview: https://YOUR-USERNAME.github.io/probite-website/

Features:
✅ Auto-scrolling product gallery
✅ Responsive design (works on all devices)
✅ Smooth animations and parallax effects
✅ Educational protein benefits section
✅ Optimized for speed and performance

Please review and let me know if you'd like any changes!

Best regards,
[Your Name]
```

---

## 📱 How Your Client Can View It

### Option 1: Direct Browser (Easiest)
1. Click the GitHub Pages link
2. That's it! Works on any device.

### Option 2: Download & Open Locally
1. On GitHub repository page, click **"Code"** → **"Download ZIP"**
2. Extract the ZIP file
3. Double-click `index.html`
4. Opens in their default browser

---

## 🔄 Making Updates After Deployment

When you make changes to the website:

```bash
# Navigate to project
cd "/Users/asif/cursor projects/Mj/ProBites"

# Make your changes to index.html or images

# Stage changes
git add .

# Commit with message
git commit -m "Update: [describe what you changed]"

# Push to GitHub
git push

# GitHub Pages auto-updates in 1-2 minutes!
```

---

## ⚙️ Custom Domain (Optional)

If your client wants a custom domain like `www.probite.com`:

1. Buy domain from provider (Namecheap, GoDaddy, etc.)
2. In GitHub repository: Settings → Pages → Custom domain
3. Add domain and follow DNS setup instructions
4. Enable HTTPS (free SSL certificate)

---

## 🆘 Troubleshooting

**Issue: "Repository not found" error**
- Check you replaced `YOUR-USERNAME` with your actual GitHub username
- Verify repository name matches exactly

**Issue: GitHub Pages shows 404**
- Wait 2-5 minutes after enabling Pages
- Check that `index.html` is in the root folder (not in a subfolder)
- Verify branch is set to `main` in Settings → Pages

**Issue: Images not loading**
- Images must be in the same folder as `index.html`
- Check capitalization of filenames (case-sensitive)

---

## 📊 Repository Stats

- **Files:** 19
- **Languages:** HTML, CSS (Tailwind), JavaScript
- **Size:** ~41MB (high-quality images)
- **Load Time:** ~2-3 seconds (first visit)

---

## ✅ Checklist Before Sharing

- [ ] Repository is public (or client has access if private)
- [ ] GitHub Pages is enabled
- [ ] Site loads correctly at the GitHub Pages URL
- [ ] Tested on mobile device
- [ ] All images display properly
- [ ] Auto-scroll gallery works
- [ ] Navigation links work
- [ ] Updated README with correct live URL

---

**Need help?** Check [GitHub Pages Documentation](https://docs.github.com/en/pages)

Good luck! 🚀
