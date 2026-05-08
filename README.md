# 🍽️ Al Maidah — Algerian · Tunisian · Syrian Cuisine
 
> *"The table that unites three nations, one spice at a time."*
 
A fully responsive, single-file restaurant website showcasing the authentic flavors of Algerian, Tunisian, and Syrian cuisine — built with pure HTML, CSS, and vanilla JavaScript. No frameworks. No dependencies. Just open and serve.
 
---
 
## ✨ Live Preview
 
Open `maghreb_table_restaurant.html` directly in any modern browser — no build step or server required.
 
---
 
## 📸 Features
 
| Feature | Details |
|---|---|
| 🌍 **Three Cuisine Layers** | Dedicated sections for Algerian 🇩🇿, Tunisian 🇹🇳 and Syrian 🇸🇾 menus |
| 🎴 **Interactive Dish Cards** | 3D tilt-on-hover effect with smooth scale and shadow transitions |
| 🎬 **Scroll Reveal Animations** | Elements animate in gracefully as you scroll down the page |
| 🏠 **Sticky Navigation** | Navbar compresses and adds shadow after scrolling 60px |
| 🦋 **Hero Floating Badges** | Animated floating dish highlights with continuous float loop |
| 📬 **Contact Form** | Validated reservation form with success feedback message |
| 📱 **Fully Responsive** | Adapts cleanly to desktop, tablet, and mobile viewports |
| 🌙 **Chef's Specials** | Highlighted promotions section on a rich terracotta background |
| 🕐 **Opening Hours Table** | Clean weekly schedule displayed in the contact section |
| 🔤 **Custom Typography** | Google Fonts: Playfair Display · Cormorant Garamond · Tajawal |
 
---
 
## 🗂️ Page Structure
 
```
Al Maidah Website
│
├── 🔝 Navigation Bar          Fixed, scroll-aware, smooth anchor links
├── 🌟 Hero Section            Animated headline, floating dish badges, CTA buttons
├── 📖 Our Story               Brand intro, stat counters, visual mosaic
│
├── 🇩🇿 Algerian Cuisine       6 dishes — Chakhchoukha, Couscous Kabyle, Brik,
│                              Tajine Zitoune, Chorba Frik, Zlabia & Kalb el Louz
│
├── 🇹🇳 Tunisian Cuisine       6 dishes — Lablabi, Salade Mechouia, Brik au Thon,
│                              Mloukhia, Poisson au Chermoula, Bambalouni
│
├── 🇸🇾 Syrian Cuisine         6 dishes — Shawarma Halabi, Kibbeh bil Sanieh,
│                              Mezze Platter, Mansaf Shami, Fattoush, Baklawa
│
├── 🔥 Chef's Specials         Friday Mechoui · Afternoon Mint Tea · Ramadan Iftar
├── 📞 Contact & Reservation   Form, phone, email, address, opening hours
└── 🦶 Footer                  Links, social icons, cuisine badges, copyright
```
 
---
 
## 🎨 Design System
 
### Color Palette
 
| Token | Hex | Usage |
|---|---|---|
| `--terracotta` | `#c4714a` | Primary accent, CTAs, borders |
| `--saffron` | `#e8a430` | Gold highlights, subtitles |
| `--cream` | `#faf6ef` | Main background |
| `--warm-white` | `#fff8f0` | Alternating section background |
| `--olive` | `#6b7c3a` | Vegetarian / fresh tags |
| `--spice` | `#8b2e1a` | Spicy / hot tags |
| `--deep-brown` | `#3a2010` | Footer background |
 
### Typography
 
| Font | Weight | Usage |
|---|---|---|
| **Playfair Display** | 400 / 600 / 900 | Headings, logo, dish names |
| **Cormorant Garamond** | 300 / 400 / 600 | Body text, descriptions |
| **Tajawal** | 300 / 400 / 700 | Labels, tags, buttons, nav |
 
---
 
## 📁 File Structure
 
```
al-maidah/
└── maghreb_table_restaurant.html   # Complete self-contained website
└── README.md                       # This file
```
 
Everything lives in a **single HTML file** — styles, scripts and markup are all co-located for maximum portability.
 
---
 
## 🚀 Getting Started
 
### Option 1 — Open directly
```bash
# Clone the repo
git clone https://github.com/your-username/al-maidah.git
 
# Open in your browser
open al-maidah/maghreb_table_restaurant.html
```
 
### Option 2 — Serve locally
```bash
# Using Python
python -m http.server 8080
 
# Using Node.js (npx)
npx serve .
```
 
Then visit `http://localhost:8080/maghreb_table_restaurant.html`
 
---
 
## 📞 Contact Details (Configured)
 
| Type | Value |
|---|---|
| 📧 Email | `thatisanarbitrayemail@gmail.com` |
| 📞 Phone | `+213 12 345 67 89` |
| 📍 Address | 12 Rue des Saveurs, Annaba, Algeria |
 
To update contact details, search for these values in the HTML file and replace them.
 
---
 
## 🛠️ Customization Guide
 
### Update restaurant name
Search for `Al Maidah` and replace with your restaurant name.
 
### Change colors
All colors are defined as CSS variables at the top of the `<style>` block:
```css
:root {
  --terracotta: #c4714a;
  --saffron: #e8a430;
  --cream: #faf6ef;
  /* ... */
}
```
 
### Add / edit dishes
Each dish follows this HTML pattern:
```html
<div class="dish-card alg">          <!-- alg | tun | syr -->
  <div class="dish-card-top">
    <div class="dish-card-bg-circle"></div>
    <div class="dish-card-emoji">🍲</div>
  </div>
  <div class="dish-card-body">
    <div class="dish-card-name">Dish Name</div>
    <div class="dish-card-desc">Description of the dish...</div>
    <div class="dish-card-footer">
      <span class="dish-price">1,400 DA</span>
      <div class="dish-tags">
        <span class="tag">Tag</span>
        <span class="tag spicy">Spicy</span>
        <span class="tag veg">Veg</span>
      </div>
    </div>
  </div>
</div>
```
 
### Update opening hours
Find the `.contact-hours` section and edit the `.hour-row` entries:
```html
<div class="hour-row">
  <span class="day">Monday – Thursday</span>
  <span class="time">11:00 – 22:30</span>
</div>
```
 
---
 
## 📱 Responsive Breakpoints
 
| Breakpoint | Behavior |
|---|---|
| `> 1024px` | Full desktop layout, floating hero badges visible |
| `≤ 1024px` | Two-column grids, hero badges hidden |
| `≤ 768px` | Single-column layout, mobile nav (links hidden) |
| `≤ 480px` | Single-column dish cards |
 
---
 
## 🌐 Browser Compatibility
 
| Browser | Support |
|---|---|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari | ✅ Full |
| Mobile Chrome | ✅ Full |
| Mobile Safari | ✅ Full |
 
Requires: `IntersectionObserver` API (supported in all modern browsers).
 
---
 
## 📄 License
 
This project is open source and available under the [MIT License](LICENSE).
 
---
 
## 🙏 Acknowledgements
 
- Fonts by [Google Fonts](https://fonts.google.com)
- Cuisine inspiration from the rich culinary traditions of Algeria, Tunisia and Syria
- Built with ❤️ and a love for good food
---
 
*Al Maidah — المائدة — The Table*
