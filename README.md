# ⬡ FieldScope — Property Damage Estimator

AI-powered property damage estimator. Takes a photo or description of damage and generates a floor plan sketch + Xactimate-style estimate.

---

## Deploy to Render.com (Free)

### Step 1 — Push to GitHub
1. Go to github.com and create a free account if you don't have one
2. Click **New Repository**, name it `fieldscope`, make it **Public**, click Create
3. Upload these files: `server.js`, `package.json`, and the `public/` folder

### Step 2 — Deploy on Render
1. Go to **render.com** and sign up for free
2. Click **New → Web Service**
3. Connect your GitHub account and select the `fieldscope` repo
4. Fill in these settings:
   - **Name:** fieldscope
   - **Runtime:** Node
   - **Build Command:** `npm install`
   - **Start Command:** `npm start`
5. Click **Add Environment Variable**:
   - Key: `ANTHROPIC_API_KEY`
   - Value: your Anthropic API key from console.anthropic.com
6. Click **Create Web Service**

### Step 3 — Share the link
Render gives you a URL like `https://fieldscope.onrender.com`
Share that with anyone — they don't need an API key!

---

## Cost
- Render free tier: $0/month
- Anthropic API: ~$0.01–0.03 per estimate (you pay, not your users)
- Set a spending limit at console.anthropic.com to control costs

## Files
- `server.js` — Node.js proxy server (keeps your API key secret)
- `package.json` — dependencies
- `public/index.html` — the FieldScope app
