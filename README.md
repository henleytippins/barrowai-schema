# Barrow-AI AEO Schema Builder

## Deploy to Vercel (10 minutes)

### Step 1 — Upload to GitHub
1. Go to github.com and create a new repository (name it `barrowai-schema`)
2. Upload this entire folder — drag the files in or use GitHub Desktop
3. Make sure the structure looks like this:
   ```
   api/
     chat.js
   public/
     index.html
   vercel.json
   README.md
   ```

### Step 2 — Connect to Vercel
1. Go to vercel.com and sign up (free) with your GitHub account
2. Click "Add New Project"
3. Import your `barrowai-schema` repository
4. Leave all build settings as default — Vercel auto-detects everything
5. Click "Deploy"

### Step 3 — Add your Anthropic API key
1. In Vercel, go to your project → Settings → Environment Variables
2. Add a new variable:
   - **Name:** `ANTHROPIC_API_KEY`
   - **Value:** your key from console.anthropic.com (starts with sk-ant-)
3. Click Save
4. Go to Deployments → click the 3 dots on your latest deployment → Redeploy

### Done!
Your app is live at `https://your-project-name.vercel.app`

---

## How it works
- `public/index.html` — the full React frontend
- `api/chat.js` — a serverless function that proxies requests to Anthropic
- Your API key stays secret on the server, never exposed to the browser
