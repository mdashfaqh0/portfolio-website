# Themed Portfolio - Customization Guide

A game-inspired, retro-styled portfolio website with GSAP animations, Framer Motion effects, and a pixel-art aesthetic.

---

## �️ Technologies Used

### Languages

| Language | Usage |
|----------|-------|
| **HTML5** | Structure of the page (`portfolio.html`) |
| **CSS3** | Styling with Tailwind CSS v4.1.13, custom properties, animations |
| **JavaScript (ES6+)** | React application logic, bundled/minified |

### Frameworks & Libraries

| Technology | Version | Purpose |
|------------|---------|---------|
| **React** | 18.x | UI component framework |
| **Tailwind CSS** | v4.1.13 | Utility-first CSS framework |
| **GSAP** | - | Advanced animations & scroll effects |
| **Framer Motion** | - | React animation library |

### Key Features

- **CSS Custom Properties** - Theme colors (`--primary`, `--secondary`, etc.)
- **CSS Layers** - `@layer base`, `@layer components`
- **React Hooks** - `useState`, `useEffect`, `useRef`, `useImperativeHandle`, `forwardRef`
- **Audio API** - HTML5 Audio for background music with fade effects
- **Responsive Design** - Mobile-first with breakpoints

### Build Type

This is a **production-bundled** single-file application - all React, CSS, and JS are compiled and minified into one HTML file (built with Vite).

---

## �📁 File Structure

```
portfolio.html    # Single-page application with embedded CSS & JS
assets/           # Images, audio, and media files
```

---

## 🎨 Theme Colors (Line 1446)

Edit the CSS custom properties in the `:root` section to change the color scheme:

| Variable       | Default Value | Description              |
|----------------|---------------|--------------------------|
| `--background` | `#fff7b3`     | Page background (yellow) |
| `--primary`    | `#ff7e00`     | Primary accent (orange)  |
| `--secondary`  | `#6a7377`     | Secondary text (gray)    |
| `--dark`       | `#2a2a2a`     | Dark text/borders        |
| `--highlight`  | `#ffce00`     | Highlight color (gold)   |
| `--light`      | `#fff`        | Light background         |

## 🚀 Quick Edit Checklist

1. **Personal Info**: Lines 20645, 20669
2. **Skills**: Lines 20541, 26225-26248
3. **Stats**: Lines 26250-26263
4. **Projects**: Lines 27170-27196
5. **Experience**: Lines 26600-26638
6. **Testimonials**: Lines 27447-27466
7. **Email**: Lines 28249, 27963
8. **Colors**: Line 1446
9. **Images**: Lines 20415, 26223, 27166-27168, 27700

---

## 📝 Notes

- This is a bundled single-file application (React + Vite build)
- All JavaScript is minified but editable
- CSS uses Tailwind v4 with custom properties
- Animations powered by GSAP and Framer Motion
- The file is ~29,000 lines due to bundled libraries

---
