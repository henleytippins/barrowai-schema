# Barrow-AI — Full Site

## Structure
```
index.html        ← Marketing homepage (barrow-ai.com)
app/
  index.html      ← Schema Builder (barrow-ai.com/app)
  tracker.html    ← Agency Tracker (barrow-ai.com/app/tracker.html)
api/
  chat.js         ← Anthropic proxy
vercel.json
```

## Deploy
1. Upload contents to GitHub repo
2. Connect to Vercel → Deploy
3. Add env var: ANTHROPIC_API_KEY = sk-ant-...
4. In Vercel: Settings → Domains → add barrow-ai.com
5. Update DNS at your registrar: CNAME @ → cname.vercel-dns.com

## Connect your domain
Vercel → Project → Settings → Domains → Add Domain → barrow-ai.com
Follow the DNS instructions shown — usually takes 5-30 min to propagate.
