# 🚀 MediPoster - Quick Deploy Guide

## ⚡ 2-Minute Setup

### 1️⃣ Push to GitHub

```bash
# Clone or download this folder
cd medi-poster

# Initialize git
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/medi-poster.git
git push -u origin main
```

### 2️⃣ Deploy on Netlify (Pick ONE)

#### **Option A: GitHub + Netlify (Recommended)**
1. Go to https://app.netlify.com
2. Click "New site from Git"
3. Connect GitHub
4. Select `medi-poster` repo
5. Settings auto-fill
6. Click "Deploy site"
7. **Done!** Your URL: `medi-poster-XXXX.netlify.app`

#### **Option B: Drag & Drop**
1. Go to https://app.netlify.com/drop
2. Drag entire `medi-poster` folder
3. **Done!** Instant deploy

#### **Option C: Vercel**
1. Go to https://vercel.com
2. Click "New Project"
3. Import GitHub repo
4. Click "Deploy"
5. **Done!**

---

## ✅ Verify It Works

- Open your URL in browser
- Fill form with test data
- Click "Export JSON" - should show data
- Click "Copy for AI" - should copy prompt
- Paste into Claude/ChatGPT to generate poster

---

## 🔑 Environment Setup (Netlify Secrets - Optional)

For GitHub Actions auto-deploy:

1. Go to Netlify Site Settings → API
2. Generate "New access token"
3. Copy token
4. Go to GitHub Repo → Settings → Secrets
5. Add secret: `NETLIFY_AUTH_TOKEN = [your-token]`
6. Add secret: `NETLIFY_SITE_ID = [from-netlify-url]`

---

## 📝 Customize

Edit `index.html` to change:
- App name/branding
- Form fields
- Colors (line ~54)
- Text content

---

## 🎯 Project Structure

```
medi-poster/
├── index.html      ← Main app (edit here)
├── package.json    ← Dependencies
├── netlify.toml    ← Netlify config
├── vercel.json     ← Vercel config
├── README.md       ← Full docs
└── LICENSE         ← MIT
```

---

## ❓ Troubleshooting

**"404 Error" on deploy?**
- netlify.toml/vercel.json present? ✓
- index.html in root? ✓
- Clear browser cache

**Form not working?**
- Open DevTools (F12)
- Check Console tab for errors
- JavaScript enabled? ✓

**Want custom domain?**
- Netlify Site Settings → Domains
- Add your domain
- Update DNS records

---

## 🚀 Next Steps

1. ✅ Deploy app
2. ✅ Test form
3. ✅ Use with Claude/ChatGPT
4. ✅ Generate posters
5. ✅ Share link with team

---

**Questions?** Check README.md for full documentation
