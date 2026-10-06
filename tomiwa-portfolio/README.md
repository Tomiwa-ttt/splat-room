# Tomiwa Ajibola portfolio

Static site (one index.html) plus one optional serverless function for live AI chat.

## Files
- index.html      the whole site (CSS, JS and images are inside it)
- favicon.svg     browser tab icon
- og.jpg          preview image when the link is shared on LinkedIn, Slack, iMessage
- api/ask.js      optional: live AI answers for "Ask my portfolio" (Vercel only)

Without api/ask.js working, the chat still answers from the built-in FAQ.

## Deploy on Vercel (recommended)
1. Create a GitHub repo (for example `portfolio`) and upload everything in this folder.
2. vercel.com > Add New > Project > import the repo > Framework preset: Other > Deploy.
3. Live chat (optional): Project > Settings > Environment Variables
   - ANTHROPIC_API_KEY = your key from console.anthropic.com
   - Set a monthly spend limit in the Anthropic console first.
   Redeploy. The chat badge changes from "Quick answers" to "Live AI answers".
4. Domain: Project > Settings > Domains > add yourdomain.com and follow the DNS records shown.

## Update later
Replace index.html in the repo and push. Vercel redeploys automatically.
