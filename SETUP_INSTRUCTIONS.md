# 🚀 GITHUB PAGES SETUP - STEP BY STEP

## BEFORE YOU START

You need:
1. A GitHub account (free) → https://github.com/join
2. These files (you have them!)
3. 10 minutes of time

---

## STEP 1: CREATE GITHUB ACCOUNT

1. Go to https://github.com/join
2. Enter your email
3. Create password
4. Choose username (this will be in your URL)
5. Verify account
6. Click "Create account"

---

## STEP 2: CREATE REPOSITORY

1. Click green "+" button (top right)
2. Select "New repository"
3. Repository name: `mziyonke-driving-school`
4. Description: `Student management system`
5. Select **Public** (required for free hosting)
6. Check ☑️ "Add a README file"
7. Click **Create repository**

---

## STEP 3: UPLOAD FILES

### Method A: Web Upload (Easiest)

1. In your new repository, click "Add file" dropdown
2. Select "Upload files"
3. Drag and drop ALL files from this folder:
   - index.html
   - mziyonke_dashboard.html
   - README.md
   - _config.yml
   - .nojekyll
   - CNAME
4. Scroll down, click "Commit changes"

### Method B: GitHub Desktop

1. Download GitHub Desktop: https://desktop.github.com
2. Clone your repository
3. Copy files to the folder
4. Commit and push

---

## STEP 4: ENABLE GITHUB PAGES

1. In your repository, click **Settings** tab
2. Scroll down to **Pages** section (left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Under "Branch", select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**
6. Wait 2-5 minutes for deployment

---

## STEP 5: ACCESS YOUR SITE

Your site will be at:
```
https://[your-username].github.io/mziyonke-driving-school/
```

Example:
- Username: `johndoe`
- URL: `https://johndoe.github.io/mziyonke-driving-school/`

You can find the exact URL in the GitHub Pages settings.

---

## STEP 6: TEST EVERYTHING

1. Open your URL in browser
2. Login with:
   - Username: `admin`
   - Password: `admin2024`
3. You should see the dashboard
4. Try adding a test student
5. Check that data persists on refresh

---

## STEP 7: SECURE YOUR SYSTEM (IMPORTANT!)

### Change Default Passwords

1. In GitHub, click on `index.html`
2. Click pencil icon (Edit)
3. Find the USERS object (around line 200)
4. Change passwords:

```javascript
const USERS = {
  'admin': { 
    password: 'your-secure-password-here',  // CHANGE THIS!
    role: 'admin',
    name: 'Administrator',
    branch: 'all'
  }
  // ... change others too
};
```

5. Scroll down, click "Commit changes"
6. Wait 2 minutes for update

---

## STEP 8: SHARE WITH YOUR TEAM

Send this to your staff:

```
🚗 Mziyonke Driving School System

URL: https://[your-username].github.io/mziyonke-driving-school/

Login Credentials:

Admin (Full Access):
- Username: admin
- Password: [your-new-password]

Staff (Branch Only):
- Username: goldspot
- Password: [your-new-password]

Instructions:
1. Open the URL
2. Login with your credentials
3. Start managing students!

For help, contact [your-name]
```

---

## 🎨 CUSTOMIZATION OPTIONS

### Add Your Logo

1. Upload logo to repository (PNG/JPG)
2. Edit `index.html`
3. Find: `src="" alt="Logo"`
4. Replace with: `src="your-logo.png"`
5. Commit changes

### Change Colors

Edit the CSS in `mziyonke_dashboard.html`:
- Primary color: `#667eea` (purple)
- Success: `#28a745` (green)
- Danger: `#dc3545` (red)

### Custom Domain

1. Buy domain (Namecheap ~R150/year)
2. In repository, edit `CNAME` file
3. Add: `www.yourschool.co.za`
4. In GitHub Pages settings, add custom domain
5. Configure DNS (instructions in GitHub)

---

## 🔒 SECURITY CHECKLIST

- [ ] Changed all default passwords
- [ ] Made repository Public (required)
- [ ] Tested on mobile device
- [ ] Shared correct URL with staff
- [ ] Bookmarked URL in office computers
- [ ] Set up backup routine (export data weekly)

---

## 🆘 TROUBLESHOOTING

### "404 File Not Found"
- Wait 5 minutes after first deploy
- Check repository is Public
- Ensure files are in main branch

### "Page Not Loading"
- Check GitHub Pages is enabled
- Try: https://[username].github.io/mziyonke-driving-school/index.html
- Clear browser cache

### "Can't Login"
- Username is case-sensitive (all lowercase)
- Check password was saved correctly
- Try incognito/private mode

### "Data Not Saving"
- GitHub Pages is static hosting (no server)
- Data saves to browser localStorage
- Each device has separate data
- Use same computer for consistent data

---

## 📞 NEED HELP?

Common issues:
1. **Forgot password**: Edit index.html in GitHub
2. **Lost data**: Check browser didn't clear storage
3. **Slow loading**: Normal for first load, caches after
4. **Mobile issues**: Should work, but desktop recommended

---

## ✅ SUCCESS!

Your system is now live and accessible from anywhere!

Next steps:
- Train staff on how to use
- Set up regular data export schedule
- Consider upgrading to database backend for multi-device sync

**🎉 Congratulations on your new system!**
