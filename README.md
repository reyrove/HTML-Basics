# 🍽️ HTML Basics — The Magical HTML Kitchen

A whimsical, food-themed guide to learning **HTML fundamentals**. Each chapter pairs a core HTML concept with a delicious dish metaphor — from "HTML Elements Soup" to "Semantic Sushi" — making the journey through web structure both memorable and fun.

> "All tags closed, all rights reserved." — Reyrove

---

## 📖 What's Inside

Nine chapters, each covering a foundational HTML topic with a culinary twist:

| # | Chapter | Dish Metaphor | Concept |
|---|---------|---------------|---------|
| 1 | The Alchemist's Table | 🍲 HTML Elements Soup | Understanding HTML elements |
| 2 | Setting Up Your Cauldron | ☕ Developer's Brew | Dev environment & browser console |
| 3 | The Magical Scroll | 🥧 HTML Structure Quiche | Page structure with semantic tags |
| 4 | The Enchanted Potions | 🍝 HTML Formatting Pasta | Text formatting & links |
| 5 | Mystical Symbols | 🍛 HTML Navigation Stew | Lists & navigation menus |
| 6 | The Wizard's Chest | 🥘 HTML Multimedia Casserole | Images, video & audio |
| 7 | Crafting with Forms | 🍔 HTML Form Burger | Forms & user input |
| 8 | The Sacred Seal | 🍣 HTML Semantic Sushi | Semantic elements & accessibility |
| 9 | The Responsive Incantations | 🥢 HTML5 & CSS Stir-Fry | Responsive design with HTML5 + CSS |

---

## 🚀 Getting Started

### 1. Clone or download

```bash
git clone https://github.com/reyrove/html-basics.git
cd html-basics
```

Or simply download the ZIP and extract it.

### 2. Project structure

```
html-basics/
├── index.html          # Main page — all 9 chapters
├── meals.css           # All styling (dark theme, responsive)
├── meals.js            # Back-to-top button behavior
├── README.md
└── images/
    ├── fav.svg         # Favicon
    ├── meal1.png       # Chapter 1 illustration
    ├── meal2.png       # Chapter 2 illustration
    ├── ...
    └── meal9.png       # Chapter 9 illustration
```

> ⚠️ **Important:** All chapter images **must** be placed inside the `images/` folder with the exact filenames shown above (`meal1.png` … `meal9.png`, lowercase). Filenames are case-sensitive on Linux and GitHub Pages.

### 3. Open it

Just double-click `index.html`, or serve it locally:

```bash
# Python 3
python -m http.server 8000

# or Node.js (npx)
npx serve .
```

Then visit `http://localhost:8000`.

---

## ✨ Features

- 🎨 **Dark theme** with a warm red accent — easy on the eyes for long reading sessions
- 📱 **Fully responsive** — layouts adapt gracefully from desktop to small phones
- 🔝 **Smooth "Top" button** — appears after scrolling 300px, gently glides back to the top
- 📖 **Semantic HTML** — the site practices what it teaches (`<header>`, `<section>`, `<footer>`, etc.)
- 🖨️ **Code samples** — every chapter includes copy-friendly `<pre><code>` snippets
- 🍽️ **Food metaphors** — complex concepts explained through relatable cooking analogies

---

## 🛠️ Tech Stack

- **HTML5** — semantic markup
- **CSS3** — custom properties, Flexbox, media queries
- **Vanilla JavaScript** — no frameworks, just a small enhancement for the back-to-top button
- **Google Fonts** — Playfair Display & Raleway
- **Font Awesome** & **Material Design Icons** — loaded for potential icon use

No build step. No dependencies to install. It just works.

---

## 🎨 Customization

### Change the accent color

In `meals.css`, find the red shades and replace them:

```css
/* Current accent */
color: #ff4d4d;          /* headings, links, code */
background: #ff4d4d;     /* back-to-top button */

/* Hover / darker shade */
color: #b30000;
background: #b30000;
```

### Change the background

```css
body {
    background-color: #1a1a1a;   /* page background */
}

.chapter {
    background-color: #1a1a1a;   /* chapter card */
    border: 1px solid #444444;   /* chapter border */
}
```

### Adjust the back-to-top trigger distance

In `meals.js`:

```js
backToTopButton.classList.toggle('show', scrollTop > 300);
//                                               ^^^ change this
```

---

## 📝 Adding a New Chapter

1. Copy an existing `<section class="chapter">` block in `index.html`.
2. Update the `<h1>`, `<p>` subtitle, and `<img src="images/mealN.png">`.
3. Add your content inside `<div class="content">`.
4. Drop the new image into `images/` (e.g., `meal10.png`).
5. Done — CSS and JS handle the rest automatically.

---

## ♿ Accessibility Notes

The site follows good semantic HTML practice:

- `<header>`, `<main>`-like structure, `<footer>` for landmark regions
- `<img>` tags include descriptive `alt` attributes
- The back-to-top button has an `aria-label`
- Color contrast (red `#ff4d4d` on dark `#1a1a1a`) meets WCAG AA for large text

If you extend the site, keep labels on form inputs, use real `<button>` elements, and preserve heading hierarchy (`h1` → `h2` → `h3`).

---

## 🧠 Learning Goals

This project is a **teaching aid**, not a production app. By reading through it (and its source), you'll encounter:

- Real-world use of semantic HTML5 elements
- CSS Flexbox for layout
- Media queries for responsive design
- CSS custom properties for theming
- Progressive enhancement with vanilla JS
- Accessible markup patterns

---

## 📄 License

© 2025–2026 **Reyrove**. All tags closed, all rights reserved.

This project is shared for learning purposes. Please credit the author if you fork or adapt it.

---

## 🙏 Credits

- Recipes, metaphors, and code — **Reyrove**
- Fonts — [Google Fonts](https://fonts.google.com/)
- Icons — [Font Awesome](https://fontawesome.com/) & [Material Design Icons](https://materialdesignicons.com/)
- Inspiration — every developer who ever compared code to cooking 🍳

---

## 💬 Feedback

Found a bug? Have a better food metaphor? Open an issue or reach out:

- 🌐 Website: [reyrove.github.io](https://reyrove.github.io/)
- 💼 LinkedIn: [Reyrove](https://www.linkedin.com/feed/update/urn:li:ugcPost:7357186806821326848/)

Happy cooking — I mean, coding! 🧑‍🍳💻
```