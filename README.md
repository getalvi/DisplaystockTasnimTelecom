# 📱 DisplayStock — Mobile Display Inventory System

A clean two-page inventory system for mobile display shops.  
Built for **GitHub Pages** hosting — no backend required.

---

## 📁 File Structure

```
/
├── index.html        ← Customer search page (public)
├── admin.html        ← Admin dashboard (password protected)
├── inventory.json    ← Inventory data (edit via admin, commit to update)
└── README.md
```

---

## 🚀 Deploy to GitHub Pages

1. **Create a GitHub repository** (can be public or private)
2. **Upload all 3 files**: `index.html`, `admin.html`, `inventory.json`
3. Go to **Settings → Pages → Source: main branch / root**
4. Your site will be live at:
   - Customer: `https://yourusername.github.io/yourrepo/`
   - Admin:    `https://yourusername.github.io/yourrepo/admin.html`

---

## 🔐 Updating Inventory (Admin Workflow)

1. Open `admin.html` → Log in
2. Add, edit, or delete items as needed
3. Click **"Download inventory.json"**
4. **Commit the new `inventory.json`** to GitHub
5. Customer page auto-refreshes with new data ✅

---

## 🔑 Changing Admin Password

Open `admin.html` and find these lines near the top of the `<script>`:

```js
const ADMIN_USER = 'admin';
const ADMIN_PASS = 'display@2025';   // ← Change this!
```

Change to a strong unique password before going live.

---

## ✨ Features

| Feature | Details |
|---|---|
| Customer search | Live filtering by brand or model name |
| Admin login | Session-based, password protected |
| CRUD | Add, edit, delete inventory items |
| Stats dashboard | Total, available, out-of-stock, units |
| JSON export | Download updated inventory for GitHub commit |
| Mobile friendly | Responsive on all screen sizes |
| No backend | 100% static — works on GitHub Pages |

---

## 🧩 How Data Flows

```
Admin types data → Saved to localStorage → Exported as JSON
→ Committed to GitHub → Customer page fetches inventory.json → Shows results
```

---

*Built with HTML, CSS, and vanilla JavaScript. No frameworks required.*
