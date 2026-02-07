# KimJoonie.github.io
My digital products store and blog

## 🛍️ Digital Products Store

A professional static website for selling digital products with Google AdSense integration.

### Features

- ✨ Modern, responsive design
- 📱 Mobile-friendly layout
- 💳 Product showcase with pricing
- 📊 Google AdSense integration ready
- 🎨 Professional styling with CSS
- ⚡ Fast loading static site
- 🔍 SEO optimized

### Products Available

The store showcases various digital products including:
- Business Template Pack
- Web Design Kit
- Social Media Graphics
- Productivity Planner
- eBook Publishing Guide
- Email Marketing Templates

### Google AdSense Setup

To activate Google AdSense on this site:

1. **Sign up for Google AdSense** at https://www.google.com/adsense/
2. **Get your Publisher ID**: After approval, you'll receive a publisher ID like `ca-pub-XXXXXXXXXXXXXXXX`
3. **Update the HTML**: Replace all instances of `ca-pub-XXXXXXXXXXXXXXXX` in `index.html` with your actual publisher ID
4. **Update Ad Slots**: Replace the example ad slot IDs (`1234567890`, `0987654321`) with your actual ad slot IDs from AdSense
5. **Verify**: Google will verify your site ownership before displaying ads

#### Ad Placements

The site includes strategic ad placements:
- Top banner ad (below hero section)
- In-feed horizontal ad (between products and about section)

### Deployment

This site is designed to work with GitHub Pages:

1. Push your changes to the repository
2. Enable GitHub Pages in repository settings
3. Select the main branch as the source
4. Your site will be live at `https://kimjoonie.github.io`

### Customization

#### Updating Products

Edit the product cards in `index.html` to add, remove, or modify products. Each product card includes:
- Product name
- Description
- Features list
- Price
- Buy button

#### Styling

Customize colors and styles in `styles.css`. Key variables are defined at the top:
```css
:root {
    --primary-color: #0066cc;
    --secondary-color: #ff6600;
    --text-color: #333;
    /* ... more variables */
}
```

#### Payment Integration

To enable actual purchases, integrate a payment processor like:
- Stripe
- PayPal
- Gumroad
- Paddle

Add the payment links to the "Buy Now" buttons.

### License

© 2026 Digital Store. All rights reserved.
