# Deployment Instructions for GitHub Pages

## 🚀 Website Information
- **Target URL:** https://rwfraser.github.io/OutskillTravelAppPrepSite
- **Repository:** https://github.com/rwfraser/OutskillTravelApp
- **Branch:** main

## 📋 Deployment Steps

### Step 1: Enable GitHub Pages

1. Go to your repository on GitHub: https://github.com/rwfraser/OutskillTravelApp

2. Click on **Settings** (gear icon) in the top navigation

3. Scroll down to the **Pages** section in the left sidebar

4. Under **Source**, select:
   - **Branch:** `main`
   - **Folder:** `/OutskillTravelApp` (or `/root` if files are in root)
   - Click **Save**

5. GitHub will display a message: "Your site is ready to be published at https://rwfraser.github.io/OutskillTravelApp/"

### Step 2: Wait for Deployment

- GitHub Pages takes 1-3 minutes to build and deploy your site
- You'll see a green checkmark when it's live
- If there's an issue, you'll see a yellow or red indicator

### Step 3: Verify Deployment

Visit your site at:
```
https://rwfraser.github.io/OutskillTravelApp/
```

Or if you want the custom path:
```
https://rwfraser.github.io/OutskillTravelAppPrepSite/
```

### Step 4: (Optional) Custom Path Setup

If you want the URL to be **OutskillTravelAppPrepSite** instead of **OutskillTravelApp**:

**Option A: Rename the Repository**
1. Go to Settings > General
2. Change repository name to: `OutskillTravelAppPrepSite`
3. Your site will be at: `https://rwfraser.github.io/OutskillTravelAppPrepSite/`

**Option B: Create a New Repository**
1. Create a new repository named `OutskillTravelAppPrepSite`
2. Push your code there instead
3. Enable GitHub Pages on that repository

## 📁 File Structure

Your deployed site includes:
```
OutskillTravelApp/
├── index.html              # Home page with green gradient
├── members.html            # Team members page (10 placeholders)
├── workbook.html           # Project workbook with 3 phases
├── about.html              # Coming Soon page
├── CompetitiveAnalysis.html      # Dark theme analysis
├── CompetitiveAnalysis_v2.html   # Light theme analysis
├── dark-theme.css          # Dark theme stylesheet
├── styles.css              # Light theme stylesheet
├── CompetitiveAnalysis.json      # Data file
└── README.md               # Documentation
```

## 🔧 Troubleshooting

### Site Not Loading
- **Check GitHub Pages Settings:** Ensure Pages is enabled
- **Wait:** Deployment can take up to 10 minutes
- **Check Actions Tab:** Look for any failed builds

### 404 Error
- Verify the branch and folder are set correctly
- Make sure `index.html` exists in the specified folder
- Files may be in `OutskillTravelApp/` subfolder - adjust path accordingly

### Styles Not Loading (Tailwind CSS)
- ✅ No issue - Tailwind is loaded via CDN in all HTML files
- Each page has: `<script src="https://cdn.tailwindcss.com"></script>`

### Links Not Working
- All links use relative paths and should work automatically
- Example: `href="members.html"` works from any page

## 🔄 Updating the Site

To make changes:

1. **Edit files locally**
   ```bash
   # Edit any .html files
   ```

2. **Commit changes**
   ```bash
   git add .
   git commit -m "Update website content"
   ```

3. **Push to GitHub**
   ```bash
   git push origin main
   ```

4. **Wait for automatic deployment** (1-3 minutes)

## ✅ Testing Checklist

After deployment, test these pages:
- [ ] Home page loads with green gradient
- [ ] Navigation menu works on all pages
- [ ] Dropdown menu (Competitors) functions properly
- [ ] Members page shows 10 placeholder cards
- [ ] Workbook accordion sections expand/collapse
- [ ] About page shows "Coming Soon"
- [ ] CompetitiveAnalysis.html loads (dark theme)
- [ ] CompetitiveAnalysis_v2.html loads (light theme)
- [ ] Site is responsive on mobile devices
- [ ] All buttons and links work

## 📱 Mobile Responsive

All pages are built with Tailwind CSS and are fully responsive:
- **Mobile:** < 640px
- **Tablet:** 640px - 1024px
- **Desktop:** > 1024px

## 🎨 Features

### Navigation
- Consistent across all pages
- Active page indicator (green underline)
- Dropdown menu for Competitors section
- Hover effects on all links

### Design
- Clean, modern Tailwind CSS styling
- Light green gradient on home page
- Card-based layouts
- Smooth transitions and animations
- Professional color scheme

### Functionality
- **Workbook:** JavaScript-powered accordion
- **Members:** Hover effects on team cards
- **Responsive:** Works on all screen sizes

## 🌐 Custom Domain (Optional)

To use a custom domain like `outskilltravel.com`:

1. Buy domain from registrar (e.g., Namecheap, GoDaddy)
2. Add `CNAME` file to repository with your domain
3. Configure DNS settings at your registrar
4. Update GitHub Pages settings with custom domain

## 📧 Support

If you encounter issues:
- Check GitHub's [Pages documentation](https://docs.github.com/en/pages)
- Verify repository visibility is set to Public
- Ensure all files are committed and pushed

---

**Deployment Date:** December 2025  
**Version:** 1.0  
**Status:** ✅ Ready for Production
