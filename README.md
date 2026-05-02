# Vasanth P — Data Scientist Portfolio

A modern, responsive personal portfolio website with dark/light mode, animated particles, skill bars, project filtering, and smooth scroll animations.

## 📁 Folder Structure

```
portfolio/
├── index.html      ← Main HTML structure (all sections)
├── style.css       ← All styles, themes, responsive breakpoints
├── script.js       ← Animations, interactivity, canvas particles
└── README.md       ← This file
```

## 🚀 Running Locally

**Option 1 — Open directly (simplest):**
```bash
# Just open in browser
open index.html
# or double-click index.html in your file explorer
```

**Option 2 — VS Code Live Server (recommended):**
1. Install the "Live Server" extension in VS Code
2. Right-click `index.html` → "Open with Live Server"

**Option 3 — Python HTTP server:**
```bash
cd portfolio
python3 -m http.server 5500
# Visit http://localhost:5500
```

**Option 4 — Node (http-server):**
```bash
npm install -g http-server
cd portfolio
http-server -p 5500
# Visit http://localhost:5500
```

## ✏️ Customizing Content

| What to change | Where |
|---|---|
| Name, title, tagline | `index.html` → Hero section |
| Social links (GitHub, LinkedIn, email) | `index.html` → Contact section & Footer |
| Project titles, descriptions, GitHub links | `index.html` → Projects section `href` attributes |
| Skill percentages | `index.html` → `data-width="XX"` on `.skill-fill` elements |
| Color accent | `style.css` → `:root { --accent: #00e5bc }` |
| Resume file | Replace `href="#"` on `.btn-resume` with `href="resume.pdf"` |

## 🎨 Features

- ✅ Dark / Light mode toggle (persists via localStorage)
- ✅ Animated canvas particle background (connected nodes)
- ✅ Custom cursor with trail
- ✅ Scroll-triggered reveal animations
- ✅ Animated skill bars (fill on scroll into view)
- ✅ Counter animation for hero stats
- ✅ Project filtering (All / ML / Deep Learning / Visualization)
- ✅ 3D tilt effect on project cards
- ✅ Contact form with mock submission
- ✅ Fully mobile responsive
- ✅ Smooth scrolling navigation

## 🌐 Deploying (Free)

**GitHub Pages:**
```bash
git init
git add .
git commit -m "Portfolio"
gh repo create vasanthp-portfolio --public
git push -u origin main
# Go to repo Settings → Pages → Branch: main
```

**Netlify (drag-and-drop):**
- Visit https://app.netlify.com/drop
- Drag your `portfolio/` folder onto the page

**Vercel:**
```bash
npm i -g vercel
cd portfolio
vercel
```

## 📝 Adding Resume

1. Save your resume as `resume.pdf` inside the `portfolio/` folder
2. Update in `index.html`:
   ```html
   <!-- Change this: -->
   <a href="#" class="btn-resume" download>
   <!-- To this: -->
   <a href="resume.pdf" class="btn-resume" download>
   ```
3. Also update `.btn-resume-card` in the About section similarly.

---
Built with pure HTML, CSS & JavaScript — no frameworks, no build step needed.
