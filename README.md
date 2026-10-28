# Ember & Oak - Premium Candle Store

A single-page candle storefront built with plain HTML, CSS and vanilla JavaScript. No frameworks, no build step. Everything lives in one file.

## Features

- Product grid with category filters (Tapers, Florals, Sculptural, Gifts, Jars & Tins)
- Live search by name, scent notes or category
- Product quick-view with reviews
- Cart drawer with quantity controls (saved in localStorage)
- Checkout form with order IDs
- Free shipping above Rs 2,000, flat Rs 99 otherwise
- Order status tracking (Awaiting payment, Paid, Packed, Shipped, Delivered)
- Razorpay Payment Link support
- Admin panel to add, edit and delete products and manage orders
- Light and dark mode, fully responsive

## How to run

1. Download or clone this repo.
2. Open index.html in your browser.

## Host on GitHub Pages

1. Rename wickradio_com.html to index.html
2. Go to Settings > Pages
3. Select the main branch and root folder, then Save
4. Your site will be live at https://YOUR-USERNAME.github.io/YOUR-REPO/

## Note

On GitHub Pages the site runs in offline mode. Browsing, search, filters and cart work. Orders, reviews and the admin panel need a backend (database and login) and will not be saved.

## Customising

- Products: edit the DEFAULTS array in the script
- Colours: CSS variables in :root
- Shipping rule: totals() function

## Tech stack

HTML5, CSS3, Vanilla JavaScript, Google Fonts, Razorpay Payment Links

## License

MIT
