# Thokoza | Artisanal African Weaving

**Thokoza** (meaning *"Rejoice"* or *"Be Happy"*) is a high-end, minimalist digital catalog designed to market handcrafted African woven products. This project prioritizes a clean, non-generic aesthetic using an earthy palette of Ochre, Sage, and Charcoal to highlight the natural textures of the craftsmanship.

## 🌿 Project Overview

This is a static, single-page application (SPA) built for speed and simplicity. It allows customers to browse a curated collection of artisanal goods and inquire directly via WhatsApp, removing the friction of a traditional checkout process for small-scale artisanal businesses.

## ✨ Key Features

* **Boutique Design:** Eschews "generic" UI for a refined, professional look using `Playfair Display` typography and organic color tones.
* **WhatsApp Commerce:** Each product includes a direct link that pre-fills a message to the seller with the specific product name.
* **Session-Based Admin Mode:** A secure-access "Staff Mode" allows authorized users (verified by phone number) to hide or manage products directly in the browser.
* **Fully Responsive:** Optimized for mobile browsing, where the majority of WhatsApp-based commerce occurs.

## 🛠️ Tech Stack

* **HTML5:** Semantic structure for SEO and accessibility.
* **CSS3:** Custom styling using CSS Variables for easy branding updates.
* **Vanilla JavaScript:** Lightweight logic for product rendering and admin authentication.

## 🚀 Setup & Usage

1.  **Clone the repo:**
    ```bash
    git clone [https://github.com/yourusername/thokoza_static.git](https://github.com/yourusername/thokoza_static.git)
    ```
2.  **Add your images:** Place your product photos in the root directory or an `/images` folder.
3.  **Launch:** Simply open `index.html` in any modern web browser.

## 🔐 Admin Access

To access the product management features, click the **"Manage Products"** button in the navigation bar. You must log in with one of the authorized phone numbers:
* `+27704145360`
* `0680157156`

Once authenticated, "Remove" buttons will appear on each product card for the duration of your session.

## ⚙️ Configuration

To update the primary contact number or authorized staff, modify the following constants in `index.html`:

```javascript
const WHATSAPP_NUM = "27704145360"; // The number that receives inquiries
const AUTH_NUMBERS = ["+27704145360", "0680157156"]; // Authorized admin numbers
