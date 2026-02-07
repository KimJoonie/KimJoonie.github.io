# Deployment Guide

## GitHub Pages Setup

1. **Enable GitHub Pages**
   - Go to repository Settings
   - Navigate to "Pages" section
   - Select source: Deploy from branch
   - Choose branch: `copilot/create-static-website-for-digital-products` (or `main` after merge)
   - Click Save

2. **Your site will be live at:**
   ```
   https://kimjoonie.github.io
   ```

## Google AdSense Setup

### Step 1: Create AdSense Account
1. Go to https://www.google.com/adsense/
2. Sign up with your Google account
3. Submit your website for review
4. Wait for approval (usually 1-2 days)

### Step 2: Get Your Publisher ID
After approval, you'll receive a publisher ID like:
```
ca-pub-1234567890123456
```

### Step 3: Update index.html
Replace all instances of `ca-pub-XXXXXXXXXXXXXXXX` with your actual publisher ID:

```html
<!-- Before -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-XXXXXXXXXXXXXXXX"
     crossorigin="anonymous"></script>

<!-- After -->
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-1234567890123456"
     crossorigin="anonymous"></script>
```

### Step 4: Create Ad Units
1. In AdSense dashboard, create ad units
2. You'll get slot IDs like `1234567890`
3. Replace the placeholder slot IDs in index.html:
   - `data-ad-slot="1234567890"` → your actual slot ID
   - `data-ad-slot="0987654321"` → your actual slot ID

### Step 5: Verify
1. Commit and push your changes
2. Wait for GitHub Pages to rebuild (2-5 minutes)
3. Google will verify your site
4. Ads will start appearing once verified

## Payment Integration

To accept payments, integrate one of these services:

### Option 1: Stripe
1. Sign up at https://stripe.com
2. Add Stripe checkout to "Buy Now" buttons
3. Handle payment webhook events

### Option 2: Gumroad
1. Sign up at https://gumroad.com
2. Create products on Gumroad
3. Link "Buy Now" buttons to Gumroad product URLs

### Option 3: PayPal
1. Create PayPal business account
2. Generate payment buttons
3. Replace "Buy Now" buttons with PayPal buttons

## Customization Tips

### Change Colors
Edit `styles.css` CSS variables:
```css
:root {
    --primary-color: #0066cc;    /* Change to your brand color */
    --secondary-color: #ff6600;  /* Change to your accent color */
}
```

### Add/Remove Products
Edit the product cards in `index.html` inside the `products-grid` section.

### Update Contact Info
Change the email and support hours in the Contact section.

## Monitoring

### Google Analytics (Optional)
Add Google Analytics to track visitors:
1. Sign up at https://analytics.google.com
2. Get your tracking code
3. Add before `</head>` in index.html

### Check AdSense Performance
Visit AdSense dashboard to monitor:
- Page views
- Clicks
- Earnings
- Best performing ad units

## Support

For issues or questions:
- Check GitHub Pages status: https://www.githubstatus.com/
- AdSense Help: https://support.google.com/adsense
- HTML/CSS validation: https://validator.w3.org/
