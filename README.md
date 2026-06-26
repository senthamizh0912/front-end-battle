# NeuralFlow — AI-Driven Data Automation Landing Page

A premium, high-converting, responsive landing page for **NeuralFlow**, a fictional AI-driven data automation platform. Built as a single-file, dependency-free experience showcasing real-time inference, auto-orchestration, and self-healing data pipelines — wrapped in a dark, gold/saffron-accented visual language with custom motion choreography.

🔗 **Live Demo:** _add your deployed link here_
🎥 **Demo Video:** _add your drive/loom link here_

---

## ✨ Features

- **Animated Hero** — staggered word-reveal typography, typing-effect status badge, and a live canvas-based particle network background that reacts to cursor movement.
- **Custom Cursor System** — a dual cursor (dot + lagging ring) with hover-state morphing on interactive elements.
- **Animated Metrics Counters** — count-up statistics that trigger on scroll via `IntersectionObserver`.
- **Infinite Marquee** — auto-generated, seamlessly looping feature ticker.
- **Bento-Style Feature Grid** — asymmetric card layout with live mini bar-chart and worker-load visualizations, mouse-tracked spotlight hover effect.
- **Matrix-Driven Pricing Engine**
  - Toggles between **Monthly / Annual** billing cycles
  - Switches across **INR (₹) / USD ($) / EUR (€)** currencies
  - Computes final prices dynamically from a multi-dimensional configuration object (base rate × tariff × cycle discount) — no hardcoded price strings
  - Updates are scoped strictly to the price text nodes (no parent/layout re-render)
- **Scroll Reveal Animations** — staggered fade/rise-in for sections as they enter the viewport.
- **Testimonials & Social Proof Grid**
- **Fully Responsive** — fluid breakpoints down to mobile, with graceful grid reflow for feature cards, pricing tiers, and footer columns.

---

## 🛠️ Tech Stack

| Layer            | Technology                                  |
|-------------------|---------------------------------------------|
| Markup            | Semantic HTML5                              |
| Styling           | Custom CSS3 (CSS variables, Grid, Flexbox, keyframe animations) |
| Interactivity     | Vanilla JavaScript (ES6+, no framework)     |
| Graphics          | HTML5 `<canvas>` (particle network), inline SVG icons |
| Fonts             | [Inter](https://fonts.google.com/specimen/Inter) (UI text), [JetBrains Mono](https://www.jetbrains.com/lp/mono/) (labels/numerics) — loaded via Google Fonts |
| Animation Engine  | Native CSS Transitions/Keyframes + `requestAnimationFrame` (no animation libraries) |
| Build Tooling     | None — zero-dependency, zero-build static page |

> No external UI kits, component libraries, or animation runtimes (e.g. Tailwind, Framer Motion, GSAP, Radix, Shadcn) are used. Everything is hand-written vanilla CSS/JS.

---

## 📦 Installation & Setup

This is a static, single-file project with **no build step and no dependencies**.

### Option 1 — Open directly
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```
2. Open `index.html` directly in your browser:
   ```bash
   # macOS
   open index.html

   # Windows
   start index.html

   # Linux
   xdg-open index.html
   ```

### Option 2 — Serve locally (recommended, avoids canvas/font edge cases)
Using any static server, for example:

```bash
# with Node.js
npx serve .

# or with Python 3
python3 -m http.server 8000
```

Then visit `http://localhost:8000` (or the port shown) in your browser.

### Deployment
Since this is a fully static page, it can be deployed as-is to any static host:

- **Vercel** — `vercel deploy`
- **Netlify** — drag-and-drop the project folder, or `netlify deploy`
- **GitHub Pages** — push to a `gh-pages` branch or enable Pages on `main` → `/ (root)`

No environment variables, API keys, or build configuration are required.

---

## 📁 Project Structure

```
.
├── index.html      # Entire application: markup, styles, and scripts
└── README.md        # This file
```

---

## 🌐 Browser Support

Targets modern evergreen browsers (Chrome, Edge, Firefox, Safari) with support for:
- CSS `:has()` selector (used for cursor hover-state morphing)
- `IntersectionObserver`
- CSS Grid & custom properties
- HTML5 Canvas

---

## 📄 License

This project was built as a speed-run / assessment submission. Add your preferred license here (e.g. MIT) if distributing publicly.
