# 🆓 Free Website Deployment: GitHub Pages + GoDaddy

## 🎯 **What You'll Get:**
- ✅ **Free hosting** (GitHub Pages)
- ✅ **Your custom domain** (GoDaddy)
- ✅ **Professional website** live on the internet
- ✅ **Version control** for easy updates
- ✅ **SSL certificate** included

---

## 📋 **Step-by-Step Setup**

### **Step 1: Create GitHub Account & Repository**

1. **Go to GitHub.com** and create an account (free)
2. **Click "New Repository"** (green button)
3. **Repository name**: `yourusername.github.io` 
   - Replace `yourusername` with your actual GitHub username
   - Example: If your username is `mbolmer3`, name it `mbolmer3.github.io`
4. **Make it Public** (required for free hosting)
5. **Don't initialize** with README (we'll upload our own files)
6. **Click "Create Repository"**

### **Step 2: Upload Your Website Files**

#### **Option A: Using GitHub Web Interface (Easiest)**
1. In your new repository, click **"uploading an existing file"**
2. **Drag and drop** these files:
   - `index.html`
   - `styles.css`
   - `script.js`
3. **Add commit message**: "Initial website upload"
4. **Click "Commit changes"**

#### **Option B: Using Git Commands (More Professional)**
```bash
# Clone the repository
git clone https://github.com/yourusername/yourusername.github.io.git

# Copy your website files into the folder
# (Copy index.html, styles.css, script.js into the folder)

# Add and commit files
git add .
git commit -m "Initial website upload"
git push origin main
```

### **Step 3: Enable GitHub Pages**

1. **Go to repository Settings** (tab at the top)
2. **Scroll down to "Pages"** (left sidebar)
3. **Source**: Select "Deploy from a branch"
4. **Branch**: Select "main"
5. **Folder**: Leave as "/ (root)"
6. **Click "Save"**

### **Step 4: Test Your Free Site**

1. **Wait 2-5 minutes** for deployment
2. **Visit**: `https://yourusername.github.io`
3. **Your website should be live!** 🎉

---

## 🔗 **Connect Your GoDaddy Domain**

### **Step 1: Get Your GitHub Pages URL**
- Your site will be at: `https://yourusername.github.io`
- Note this URL down

### **Step 2: Update GoDaddy DNS**

1. **Log into GoDaddy** and go to your domain
2. **Click "Manage DNS"**
3. **Add/Edit DNS Records**:

#### **For Root Domain (yourdomain.com):**
- **Type**: CNAME
- **Name**: `@`
- **Value**: `yourusername.github.io`
- **TTL**: 600 (or default)

#### **For WWW (www.yourdomain.com):**
- **Type**: CNAME  
- **Name**: `www`
- **Value**: `yourusername.github.io`
- **TTL**: 600 (or default)

### **Step 3: Wait for DNS Propagation**
- **Time**: 24-48 hours (usually much faster)
- **Check**: Visit `https://www.whatsmydns.net/` to see propagation status

---

## ✅ **Verification Checklist**

- [ ] GitHub repository created: `yourusername.github.io`
- [ ] Website files uploaded to repository
- [ ] GitHub Pages enabled in repository settings
- [ ] Site accessible at: `https://yourusername.github.io`
- [ ] GoDaddy DNS records updated
- [ ] Custom domain working (after DNS propagation)

---

## 🛠️ **Troubleshooting**

### **Site Not Loading:**
1. Check repository name is exactly `yourusername.github.io`
2. Verify files are in the root of the repository
3. Wait 5-10 minutes after enabling Pages
4. Check repository is Public

### **DNS Not Working:**
1. Verify CNAME records are correct
2. Use `https://www.whatsmydns.net/` to check propagation
3. Wait 24-48 hours for full propagation
4. Clear browser cache

### **HTTPS Issues:**
1. GitHub Pages automatically provides SSL
2. Make sure you're using `https://` not `http://`
3. Wait for SSL certificate to activate (can take 24 hours)

---

## 🔄 **Updating Your Website**

### **To Make Changes:**
1. **Edit files** in your GitHub repository
2. **Commit changes** with a message
3. **Wait 2-5 minutes** for automatic deployment
4. **Your site updates automatically!**

### **Example Update Process:**
1. Go to your repository on GitHub
2. Click on `index.html`
3. Click the pencil icon to edit
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait for deployment

---

## 💡 **Pro Tips**

1. **Bookmark your repository** for easy access
2. **Use descriptive commit messages** for changes
3. **Test locally** before uploading
4. **Keep a backup** of your files locally
5. **Monitor your site** after DNS changes

---

## 🎉 **You're Done!**

Your website is now:
- ✅ **Live on the internet**
- ✅ **Using your custom domain**
- ✅ **Completely free**
- ✅ **Professional and fast**
- ✅ **Easy to update**

**Total Cost: $0** (except your domain registration)

---

## 📞 **Need Help?**

- **GitHub Support**: https://docs.github.com/en/pages
- **GoDaddy Support**: 24/7 phone and chat
- **DNS Checker**: https://www.whatsmydns.net/
- **GitHub Pages Status**: https://www.githubstatus.com/
