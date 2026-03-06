# Mziyonke Driving School - Student Management System

🚗 **Live Demo**: https://[your-username].github.io/mziyonke-driving-school/

## 📋 About

A complete student progress tracking system for driving schools with:
- ✅ Secure login system
- ✅ Role-based access (Admin/Manager/Staff)
- ✅ Multi-branch support
- ✅ Payment tracking
- ✅ WhatsApp integration
- ✅ Financial reporting
- ✅ Cloud-sync ready

## 🚀 Quick Start

### Default Logins

| Role | Username | Password |
|------|----------|----------|
| Admin | `admin` | `*********` |
| Manager | `manager` | `**********` |
| Staff | `goldspot` | `********` |

### Branches Supported
- Gold Spot (Main)
- Chris Hani
- Bara
- Protea Glen
- Dawn Park

## 🛠️ Setup Instructions

### Step 1: Fork/Create Repository

1. Go to https://github.com/new
2. Repository name: `mziyonke-driving-school`
3. Make it **Public** (for free hosting)
4. Check "Add a README file"
5. Click **Create repository**

### Step 2: Upload Files

**Option A: Drag & Drop**
1. Download this repository as ZIP
2. Extract files
3. Go to your GitHub repository
4. Click "Add file" → "Upload files"
5. Drag all files from this folder
6. Commit changes

**Option B: Git Command Line**
```bash
git clone https://github.com/[your-username]/mziyonke-driving-school.git
cd mziyonke-driving-school
# Copy all files from this folder
git add .
git commit -m "Initial setup"
git push origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll down to **Pages** section
3. Source: Select **Deploy from a branch**
4. Branch: Select **main** → **/ (root)**
5. Click **Save**
6. Wait 2-3 minutes for deployment
7. Your URL will show: `https://[username].github.io/mziyonke-driving-school/`

## 🔐 Security Notes

⚠️ **IMPORTANT**: This is a client-side application
- Data is stored in browser localStorage
- For production use, add a backend database
- Change default passwords before deploying
- Consider adding encryption for sensitive data

## 📝 Customization

### Change Passwords
Edit `index.html` and modify the USERS object:

```javascript
const USERS = {
  'admin': { 
    password: 'your-new-password',  // Change this
    role: 'admin',
    name: 'Administrator',
    branch: 'all'
  }
  // ... other users
};
```

### Add Your Logo
1. Add logo image to repository
2. Update path in HTML files

### Custom Domain (Optional)
1. Buy domain from Namecheap/GoDaddy
2. Add CNAME file to repository
3. Configure DNS settings
4. Enable HTTPS in GitHub Pages settings

## 📱 Features

### For Administrators
- View all branches
- Manage all students
- See financial summaries
- Export data to Excel

### For Managers
- View all branches
- Edit student records
- Track payments
- Generate reports

### For Staff
- View assigned branch only
- Add new students
- Update progress
- Send WhatsApp messages

## ☁️ Data Backup

Since this uses browser storage:
- Data is saved locally on each device
- To sync across devices, set up Google Sheets integration
- Regularly export data using "Export to Excel" button

## 🆘 Troubleshooting

### Can't Login?
- Check username is lowercase
- Clear browser cache (Ctrl+Shift+Delete)
- Try incognito mode

### Data Not Saving?
- Ensure localStorage is enabled
- Check browser privacy settings
- Disable "Clear cookies on exit"

### Page Not Loading?
- Check GitHub Pages is enabled in settings
- Ensure repository is public
- Wait 5 minutes after first deploy

## 📞 Support

For issues or questions:
1. Check browser console (F12) for errors
2. Review GitHub Pages deployment status
3. Test locally before deploying

## 📄 License

Free for educational use. Modify as needed for your driving school.

---

**Made with ❤️ for Mziyonke Driving School**
