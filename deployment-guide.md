# Website Deployment Guide

## 🚀 Deployment Options

### Option 1: GoDaddy Hosting (Recommended)
**Cost**: ~$5-10/month
**Pros**: Full control, good performance, easy management
**Cons**: Monthly cost

### Option 2: GitHub Pages + GoDaddy Domain (Free)
**Cost**: Free hosting + domain cost
**Pros**: Free, reliable, version control
**Cons**: Slightly more technical setup

### Option 3: Netlify + GoDaddy Domain (Free)
**Cost**: Free hosting + domain cost
**Pros**: Free, fast, easy deployment
**Cons**: Requires account setup

---

## 📋 GoDaddy Hosting Setup

### Step 1: Purchase Hosting
1. Go to GoDaddy.com → Web Hosting
2. Choose "Basic" or "Economy" plan
3. Select your domain
4. Complete purchase

### Step 2: Access File Manager
1. GoDaddy Dashboard → Web Hosting → Manage
2. Find "File Manager" or "cPanel"
3. Navigate to `public_html` folder

### Step 3: Upload Files
1. Delete default files in `public_html`
2. Upload these files:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `README.md` (optional)

### Step 4: Test
Visit your domain - site should be live!

---

## 🆓 GitHub Pages Setup (Free)

### Step 1: Create GitHub Repository
1. Go to GitHub.com
2. Click "New Repository"
3. Name it: `yourusername.github.io`
4. Make it Public
5. Don't initialize with README

### Step 2: Upload Files
1. Clone repository locally
2. Copy your website files into the folder
3. Push to GitHub:
```bash
git add .
git commit -m "Initial website upload"
git push origin main
```

### Step 3: Enable GitHub Pages
1. Repository Settings → Pages
2. Source: "Deploy from a branch"
3. Branch: "main"
4. Save

### Step 4: Connect GoDaddy Domain
1. GoDaddy DNS Management
2. Add CNAME record:
   - Name: `@` or `www`
   - Value: `yourusername.github.io`
3. Wait 24-48 hours for propagation

---

## ⚡ Netlify Setup (Free)

### Step 1: Create Netlify Account
1. Go to Netlify.com
2. Sign up with GitHub
3. Click "New site from Git"

### Step 2: Connect Repository
1. Choose GitHub
2. Select your repository
3. Deploy settings:
   - Build command: (leave empty)
   - Publish directory: (leave empty)
4. Deploy site

### Step 3: Connect Domain
1. Site Settings → Domain Management
2. Add custom domain
3. Update GoDaddy DNS:
   - Add A record pointing to Netlify IP
   - Or use Netlify's nameservers

---

## 🔧 DNS Configuration

### GoDaddy DNS Settings
1. GoDaddy Dashboard → Domains → Manage DNS
2. Add/Edit records:

**For GitHub Pages:**
- Type: CNAME
- Name: `@` or `www`
- Value: `yourusername.github.io`

**For Netlify:**
- Type: A
- Name: `@`
- Value: `75.2.60.5`

**For GoDaddy Hosting:**
- Usually automatic, but verify A record points to hosting IP

---

## ✅ Post-Deployment Checklist

- [ ] Website loads correctly
- [ ] All links work
- [ ] Images display properly
- [ ] Contact form works (if applicable)
- [ ] Mobile responsive
- [ ] SSL certificate active (https://)
- [ ] Google Analytics added (optional)
- [ ] SEO meta tags added (optional)

---

## 🛠️ Troubleshooting

### Common Issues:
1. **Site not loading**: Check DNS propagation (24-48 hours)
2. **CSS not loading**: Verify file paths are correct
3. **Images broken**: Check image file names and paths
4. **HTTPS issues**: Enable SSL in hosting control panel

### Performance Tips:
1. Compress images before uploading
2. Enable GZIP compression
3. Use a CDN for faster loading
4. Minimize CSS/JS files

---

## 📞 Support Resources

- **GoDaddy Support**: 24/7 phone and chat
- **GitHub Pages Docs**: https://pages.github.com/
- **Netlify Docs**: https://docs.netlify.com/
- **DNS Checker**: https://www.whatsmydns.net/

---

## 💡 Pro Tips

1. **Always backup** your files before making changes
2. **Test locally** before uploading
3. **Use version control** (Git) for easy updates
4. **Monitor site performance** with tools like Google PageSpeed
5. **Set up automatic backups** if using paid hosting
