# Barrow-AI AEO Platform v2

## File structure
```
api/
  chat.js          ← Anthropic proxy (serverless function)
public/
  index.html       ← Schema Builder
  tracker.html     ← Agency Tracker Dashboard
vercel.json        ← Routing config
```

## Deploy to Vercel

1. Push this folder to a GitHub repo (upload the contents, not a zip)
2. Connect repo to Vercel → Deploy
3. Add environment variable: ANTHROPIC_API_KEY = sk-ant-...
4. Redeploy

## Pages
- `/` → Schema Builder (AI interview → JSON-LD)
- `/tracker.html` → Agency Tracker (all clients, scores, alerts)

Both pages share the same sidebar nav and Barrow-AI branding.
The Schema Builder shows an "Open Tracker →" CTA after schema generation.
The Tracker shows a "New Schema →" link back to the builder.
