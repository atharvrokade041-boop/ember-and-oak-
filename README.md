# 🕯️ Ember & Oak – Premium Candle Store

A single-page, hand-poured-candle storefront built with plain **HTML, CSS and vanilla JavaScript**. No frameworks, no build step – everything lives in one file.

> Poured by hand. Lit by you.

---

## ✨ Features

**Storefront**
- Product grid with category filters: Tapers, Florals, Sculptural, Gifts, Jars & Tins
- Live search by name, scent notes or category
- Product quick-view with ratings and reviews
- Slide-out cart drawer with quantity controls (cart is saved in `localStorage`)
- Checkout form (name, phone, delivery address) with order IDs
- Free shipping above ₹2,000, flat ₹99 otherwise
- Prices in INR (₹) with Indian number formatting

**Orders & payments**
- "My orders" tab with status tracking: Awaiting payment → Paid → Packed → Shipped → Delivered
- Razorpay Payment Link support – customers get a "Pay now" button after placing an order

**Admin panel ("Atelier")**
- Add, delete and edit products (price, stock, fragrance name, photo)
- Paste your Razorpay Payment Link
- View all orders and update their status

**Design**
- Warm, editorial look (Fraunces / Karla fonts)
- Automatic light and dark mode
- Fully responsive, with safe-area support for phones
- Animated SVG candle flame as a fallback when a product has no photo

---

## 🚀 Getting started

No installation needed.

```bash
# 1. Clone the repo
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

# 2. Open the page
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Or serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

### Host it free on GitHub Pages
1. Rename `wickradio_com.html` to `index.html`
2. Go to **Settings → Pages**
3. Under **Source**, choose the `main` branch and `/ (root)`, then click **Save**
4. Your site goes live at `https://<your-username>.github.io/<your-repo>/`

---

## ⚠️ Running as a static copy

The orders, reviews and admin panel need a backend (a database, user login and file storage). When you open this file on GitHub Pages or locally, it runs in **offline mode**:

| Feature | Static copy |
|---|---|
| Browse, search, filter products | ✅ Works |
| Cart (saved in browser) | ✅ Works |
| Placing orders / order history | ❌ Not saved |
| Reviews | ❌ Not saved |
| Admin panel & Razorpay link | ❌ Hidden |

To make it fully functional, connect your own backend (e.g. Firebase, Supabase) in place of the `S.db` / `S.assets` calls in the script.

---

## 🗂️ Project structure

```
.
├── index.html   # entire app: markup, styles and scripts
└── README.md
```

The 13 sample products live in the `DEFAULTS` array inside the `<script>` tag. Edit it to change the catalog.

---

## 🛠️ Customising

| What | Where |
|---|---|
| Brand name & copy | `<header>` and `.hero` section |
| Colours / dark mode | CSS variables in `:root` |
| Products | `DEFAULTS` array in the script |
| Shipping rule | `totals()` function |
| Categories | `cats` array in `renderShop()` |

---

## 🧰 Tech stack

- HTML5
- CSS3 (custom properties, grid, flexbox, `prefers-color-scheme`)
- Vanilla JavaScript (ES6+)
- Google Fonts
- Razorpay Payment Links

---

## 📄 License

Released under the [MIT License](LICENSE). Product photos and brand name are for demonstration – replace them with your own before going live.

---

Made with 🤎 in India
