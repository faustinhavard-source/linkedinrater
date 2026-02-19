# LinkedIn Post Rater — EF Edition

AI-powered LinkedIn post analyzer for Entrepreneurs First.

## Deploy on Vercel (5 minutes)

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "init linkedin rater"
git remote add origin https://github.com/TON_USERNAME/linkedin-rater.git
git push -u origin main
```

### 2. Import on Vercel
- Go to [vercel.com](https://vercel.com) → New Project
- Import your GitHub repo
- Click **Deploy** (no build config needed)

### 3. Add your Anthropic API key
- In Vercel dashboard → Settings → Environment Variables
- Add: `ANTHROPIC_API_KEY` = `sk-ant-...`
- **Redeploy** (Settings → Deployments → Redeploy)

Done. Your app is live at `https://your-project.vercel.app`

## Project structure
```
├── api/
│   └── analyze.js      # Proxy route (keeps API key server-side)
├── public/
│   └── index.html      # Full app (single file)
├── package.json
└── vercel.json
```
