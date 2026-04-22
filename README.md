# Hearth — Family Meal Planner

Your personal AI-powered meal planning app for Sherborn, MA.

## Deploy to Vercel (20 minutes)

### Step 1: Get your Anthropic API key
1. Go to https://console.anthropic.com
2. Sign up / log in
3. Go to API Keys → Create Key
4. Copy the key (starts with `sk-ant-...`)

### Step 2: Push to GitHub
1. Create a free account at https://github.com if you don't have one
2. Create a new repository called `hearth` (keep it private)
3. Upload all files from this folder, OR run:
   ```
   git init
   git add .
   git commit -m "Hearth meal planner"
   git remote add origin https://github.com/YOUR_USERNAME/hearth.git
   git push -u origin main
   ```

### Step 3: Deploy on Vercel
1. Go to https://vercel.com and sign up with your GitHub account
2. Click "Add New Project"
3. Import your `hearth` repository
4. In "Environment Variables", add:
   - Name: `ANTHROPIC_API_KEY`
   - Value: your key from Step 1
5. Click Deploy
6. Wait ~60 seconds — you'll get a URL like `hearth.vercel.app`

### Step 4: Add to your phone home screen
**iPhone:**
1. Open your Vercel URL in Safari
2. Tap the Share button (box with arrow)
3. Tap "Add to Home Screen"
4. Name it "Hearth" → Add
5. It now lives on your home screen like an app

**Android:**
1. Open in Chrome
2. Tap ⋮ menu → "Add to Home Screen"

## That's it!
The app works on any device. Your API key stays secret on Vercel's servers.
Camera upload works natively on mobile — tap "Choose / take photos" in the Pantry tab.

## Instacart API key (when you get it)
When your Instacart Developer Platform key arrives (~4 weeks):
1. Go to Vercel → your project → Settings → Environment Variables
2. Add: `INSTACART_API_KEY` = your key
3. Redeploy
4. The "Open Instacart" button will generate real pre-populated shopping lists

## Costs
- Vercel: Free tier (plenty for personal use)
- Anthropic API: ~$5–15/month at typical family usage
  - Weekly planning session: ~$0.10
  - Fridge photo scan: ~$0.05
  - Chat messages: ~$0.01 each
