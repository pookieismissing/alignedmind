# GitHub Pages Deployment Guide

This guide will help you deploy your Aligned Mind Psychology and Wellness website to GitHub Pages for testing.

## 📋 Prerequisites

- A GitHub account (sign up at https://github.com if you don't have one)
- Git installed on your computer (download from https://git-scm.com)

## 🚀 Step-by-Step Deployment

### Option 1: Using GitHub.com (Easiest - No Git Installation Needed)

1. **Create a new repository on GitHub:**
   - Go to https://github.com/new
   - Repository name: `aligned-mind-website` (or any name you prefer)
   - Description: "Aligned Mind Psychology and Wellness Website"
   - Choose "Public" (required for free GitHub Pages)
   - Don't initialize with README, .gitignore, or license
   - Click "Create repository"

2. **Upload files:**
   - On your new repository page, click "uploading an existing file"
   - Drag and drop ALL these files:
     - index.html
     - about.html
     - services.html
     - contact.html
     - faq.html
     - practice-info.html
     - styles.css
     - script.js
   - Add commit message: "Initial website commit"
   - Click "Commit changes"

3. **Enable GitHub Pages:**
   - Go to your repository settings (click "Settings" tab)
   - Scroll down to "Pages" in the left sidebar
   - Under "Source", select "main" branch
   - Click "Save"
   - Wait 1-2 minutes for deployment

4. **View your site:**
   - Your site will be available at: `https://YOUR-USERNAME.github.io/aligned-mind-website/`
   - GitHub will show you the URL in the Pages settings

---

### Option 2: Using Git Command Line (For Advanced Users)

1. **Create repository on GitHub** (same as Option 1, step 1)

2. **Initialize local repository:**
   ```bash
   cd /path/to/your/website/files
   git init
   git add .
   git commit -m "Initial website commit"
   ```

3. **Connect to GitHub and push:**
   ```bash
   git remote add origin https://github.com/YOUR-USERNAME/aligned-mind-website.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages** (same as Option 1, step 3)

---

## 🔄 Making Updates

### Option 1 (GitHub.com):
- Go to your repository
- Click on the file you want to edit
- Click the pencil icon (Edit)
- Make changes
- Scroll down, add commit message, click "Commit changes"
- Changes will appear on your site in 1-2 minutes

### Option 2 (Git Command Line):
```bash
# Make your changes to files locally
git add .
git commit -m "Description of changes"
git push
```

---

## 🎨 Customization Before Going Live

Before sharing your site publicly, update these items:

1. **Add your logo:**
   - Upload logo file to repository
   - Update navigation in all HTML files

2. **Add professional photos:**
   - Upload images to repository
   - Update image placeholders in about.html

3. **Update Patient Portal URL:**
   - Replace `https://portal.example.com` with actual portal URL
   - Update in all HTML files

4. **Test contact form:**
   - Set up form backend (Formspree, Netlify Forms, etc.)
   - Update form action in contact.html

5. **Add Google Maps:**
   - Get embed code from Google Maps
   - Replace map placeholder in contact.html

---

## 🌐 Custom Domain (Optional)

To use your own domain (e.g., alignedmindpsych.com):

1. **Buy a domain** from:
   - Namecheap
   - Google Domains
   - GoDaddy
   - etc.

2. **Configure DNS:**
   - In your domain settings, add these records:
     ```
     A Record: 185.199.108.153
     A Record: 185.199.109.153
     A Record: 185.199.110.153
     A Record: 185.199.111.153
     CNAME Record: www → YOUR-USERNAME.github.io
     ```

3. **Update GitHub Pages:**
   - Go to repository Settings → Pages
   - Under "Custom domain", enter your domain
   - Click "Save"
   - Wait 24-48 hours for DNS propagation

---

## ✅ Testing Checklist

Before sharing your site, test:

- [ ] All navigation links work
- [ ] All pages load correctly
- [ ] Mobile responsive design works
- [ ] Forms submit properly
- [ ] Contact information is correct
- [ ] FAQ accordion works
- [ ] Practice info tabs work
- [ ] All links open in correct windows
- [ ] Site looks good on phone, tablet, and desktop

---

## 🔧 Troubleshooting

**Site not loading?**
- Wait 2-5 minutes after pushing changes
- Check repository Settings → Pages for deployment status
- Ensure repository is public

**Styles not loading?**
- Make sure styles.css is in the same directory as HTML files
- Check browser console for errors (F12)

**Links broken?**
- Verify all filenames are lowercase
- Check that all files are in the root directory

**Mobile menu not working?**
- Make sure script.js is uploaded
- Check browser console for JavaScript errors

---

## 📞 Need Help?

If you run into issues:
1. Check GitHub's documentation: https://docs.github.com/pages
2. Verify all files are uploaded correctly
3. Check browser console for errors (press F12)

---

## 🎉 You're Live!

Once deployed, your website will be accessible at:
`https://YOUR-USERNAME.github.io/aligned-mind-website/`

Share this URL for testing before setting up a custom domain!
