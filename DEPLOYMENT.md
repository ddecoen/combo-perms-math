# Deployment Instructions for Vercel

## Quick Deploy (Easiest Method)

### Option 1: Deploy via GitHub (Recommended)

1. **Push these files to your GitHub repository:**
   ```bash
   cd combo-perms-math
   cp /path/to/index.html .
   cp /path/to/vercel.json .
   git add index.html vercel.json
   git commit -m "Add combinations and permutations calculator web app"
   git push origin main
   ```

2. **Connect to Vercel:**
   - Go to [vercel.com](https://vercel.com)
   - Sign in with your GitHub account
   - Click "Add New Project"
   - Select your `combo-perms-math` repository
   - Click "Deploy"

That's it! Vercel will automatically deploy your site and give you a URL.

### Option 2: Deploy via Vercel CLI

1. **Install Vercel CLI:**
   ```bash
   npm install -g vercel
   ```

2. **Navigate to your project directory:**
   ```bash
   cd combo-perms-math
   ```

3. **Deploy:**
   ```bash
   vercel
   ```

4. **Follow the prompts:**
   - Login to Vercel (if not already logged in)
   - Confirm project settings
   - Wait for deployment to complete

### Option 3: Drag and Drop (No CLI needed)

1. Go to [vercel.com](https://vercel.com)
2. Sign in
3. Click "Add New Project"
4. Select "Import from Git" or simply drag and drop your project folder
5. Vercel will detect it's a static site and deploy automatically

## Project Structure

Your project should have these files:

```
combo-perms-math/
├── index.html       # Main calculator app
├── vercel.json      # Vercel configuration
└── README.md        # Documentation (optional)
```

## After Deployment

Once deployed, you'll get a URL like:
- `https://combo-perms-math.vercel.app`
- Or your custom domain if configured

## Custom Domain (Optional)

1. Go to your project in Vercel dashboard
2. Click "Settings" → "Domains"
3. Add your custom domain
4. Follow the DNS configuration instructions

## Automatic Deployments

When connected via GitHub, every push to your repository automatically triggers a new deployment on Vercel.

## Features of Your Web App

✅ Calculate permutations P(n, r)
✅ Calculate combinations C(n, r)
✅ Real-time validation
✅ Responsive design (works on mobile)
✅ Modern, clean UI
✅ Optimized calculations for large numbers
✅ Quick reference guide built-in

## Support

For Vercel deployment issues, visit: https://vercel.com/docs

For calculator issues, open an issue on your GitHub repository.
