# 🏥 MediPoster

Hospital and Clinic Poster Generator - Generate professional posters using AI

## Features

✨ **Simple Form** - Enter hospital/clinic details  
📋 **JSON Export** - Structured data for any AI  
🤖 **AI Ready** - Copy prompt for Claude, ChatGPT, etc.  
🎨 **Customizable** - Brand colors and images  
📱 **Responsive** - Works on mobile and desktop  

## Quick Start

### Local Development

```bash
# Install dependencies
npm install

# Run dev server
npm run dev

# Open browser
http://localhost:3000
```

### What You Get

1. **Export JSON** - Structured hospital data
2. **Copy for AI** - Auto-generates prompt with JSON embedded
3. Share with AI to generate poster designs

---

## Deploy on Netlify

### Option 1: Using GitHub (Recommended)

1. **Create GitHub Repo**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/medi-poster.git
   git push -u origin main
   ```

2. **Connect to Netlify**
   - Go to [netlify.com](https://netlify.com)
   - Click "New site from Git"
   - Select GitHub repository
   - Build command: `npm run build`
   - Publish directory: `.`
   - Click Deploy

3. **Done!** Your site is live

### Option 2: Direct Upload
- Drag & drop folder to netlify.com/drop

---

## Deploy on Vercel

1. **Push to GitHub** (see Netlify steps 1)

2. **Connect to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import GitHub repo
   - Click Deploy

3. **Done!** Site is live

---

## How to Use

### Step 1: Fill Form
- Hospital name
- Address
- Phone & Email
- Services
- Key message
- Brand color

### Step 2: Export
- Click "Export JSON" to see structured data
- Click "Copy for AI" to generate prompt

### Step 3: Share with AI
Paste the copied prompt into:
- Claude
- ChatGPT
- Gemini
- Any LLM

### Step 4: Get Poster
AI generates poster design using your data

---

## File Structure

```
medi-poster/
├── index.html          # Main app
├── server.js          # Express server
├── package.json       # Dependencies
├── netlify.toml       # Netlify config
├── vercel.json        # Vercel config
├── .gitignore         # Git ignore
└── README.md          # This file
```

---

## JSON Data Format

```json
{
  "organizationName": "City Care Hospital",
  "address": "123 Medical St, Hyderabad",
  "phone": "+91 XXXXXX",
  "email": "contact@hospital.com",
  "services": ["Emergency", "Surgery", "ICU"],
  "keyMessage": "24/7 Healthcare Excellence",
  "logoUrl": "https://example.com/logo.png",
  "brandColor": "#667eea",
  "generatedAt": "2026-06-30T..."
}
```

---

## Environment Variables

No environment variables needed. This is a static app!

---

## Custom Domain (Netlify)

1. Go to Netlify Site Settings
2. Domain settings → Add custom domain
3. Update DNS records (Netlify provides instructions)

---

## Troubleshooting

**Getting 404 error?**
- Check netlify.toml or vercel.json is present
- Ensure index.html is in root directory

**Form not working?**
- Open browser console (F12) for errors
- Check JavaScript is enabled

**Deploy failed?**
- Verify package.json exists
- Check npm install runs without errors

---

## License

MIT - Use freely for any purpose

---

## Contributing

Issues and PRs welcome! 

---

## Support

Email: support@mediposter.dev  
GitHub: github.com/YOUR_USERNAME/medi-poster

---

**Made with ❤️ for healthcare professionals**
