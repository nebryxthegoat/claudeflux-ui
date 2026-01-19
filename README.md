# ClaudeFlux - Intelligent AI Router

A beautiful, modern dashboard for intelligent AI routing that optimizes costs and performance.

## 🚀 Deployment to Vercel

### Method 1: Using Vercel CLI

1. Install Vercel CLI:
```bash
npm i -g vercel
```

2. Navigate to your project directory and run:
```bash
vercel
```

3. Follow the prompts to deploy

### Method 2: Using Vercel Dashboard

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New Project"
3. Import your Git repository
4. Vercel will automatically detect the configuration
5. Click "Deploy"

## 📁 File Structure

```
.
├── index.html          # Homepage with company info
├── analytics.html      # Analytics dashboard
├── vercel.json        # Vercel configuration
└── README.md          # This file
```

## 🔧 Configuration

The `vercel.json` file includes routing configuration to ensure:
- Root path (`/`) serves `index.html`
- `/analytics` route serves `analytics.html`
- All other paths are handled correctly

## 🌐 Navigation

- **Homepage** (`/`): Company information, features, and calls-to-action
- **Analytics** (`/analytics.html`): Real-time dashboard with metrics and statistics

## 🎨 Features

### Homepage
- Hero section with clear value proposition
- Key statistics overview
- Feature showcase (6 main features)
- How it works (4-step process)
- What we offer (6 additional services)
- Call-to-action section

### Analytics Dashboard
- Live statistics cards
- Model usage charts
- Recent activity feed
- Weekly cost breakdown
- Model performance comparison
- Interactive visualizations

## 🛠️ Customization

All colors and styling are defined in CSS variables at the top of each HTML file:

```css
:root {
    --bg-primary: #0a0e1a;
    --bg-secondary: #12182b;
    --accent-cyan: #00f5ff;
    --accent-purple: #b84fff;
    /* ... etc */
}
```

## 📱 Responsive Design

Both pages are fully responsive and work seamlessly on:
- Desktop (1920px+)
- Laptop (1366px - 1920px)
- Tablet (768px - 1366px)
- Mobile (320px - 768px)

## 🐛 Troubleshooting

### 404 Errors on Vercel

If you see 404 errors after deployment:

1. **Ensure `vercel.json` is in the root directory** of your project
2. **Check that file names match exactly**: `index.html` and `analytics.html`
3. **Use root-relative paths** for all internal links (e.g., `/analytics.html` instead of `analytics.html`)
4. **Redeploy** after making changes to `vercel.json`

### Links Not Working

If navigation links don't work:
- Make sure all internal links start with `/` (e.g., `href="/analytics.html"`)
- Check browser console for JavaScript errors
- Verify that anchor links use `#` for in-page navigation

## 📄 License

Copyright © 2025 ClaudeFlux. All rights reserved.
