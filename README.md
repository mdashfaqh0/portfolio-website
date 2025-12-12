# Themed Portfolio - Customization Guide

A game-inspired, retro-styled portfolio website with GSAP animations, Framer Motion effects, and a pixel-art aesthetic.

---

## 📁 File Structure

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

**Location:** Line 1446 (search for `:root{--background:`)

---

## 📄 Page Title (Line 6)

```html
<title>Themed Portfolio</title>
```

---

## 👤 Personal Information

### Hero Section - Name & Title (Lines 20645-20669)

| Content                | Line   | Current Value                                                                                     |
|------------------------|--------|---------------------------------------------------------------------------------------------------|
| Name words             | 20645  | `["Hi,", "I'm", "Gaurav", "—", "Dev", "&", "Creator"]`                                            |
| Bio/Tagline            | 20669  | `"I build game-inspired web experiences — heavy on performance, clean UI, and delightful micro-interactions..."` |

### Hero Skill Tags (Line 20541)

```javascript
p = ["React", "TypeScript", "Framer Motion", "Tailwind", "3D / Assets"]
```

### Hero Featured Cards (Lines 20543-20563)

```javascript
g = [{
    title: "Top Project",
    subtitle: "GTA Mod UI",
    rotate: 2,
    delay: .08
}, {
    title: "Live",
    subtitle: "GTA6 launch plan",
    ...
}]
```

---

## 🧭 Navigation Links

### Desktop Navigation (Lines 20278-20296)

```javascript
const NR = [{
    href: "#home",
    label: "Home"
}, {
    href: "#about",
    label: "About"
}, {
    href: "#skills",
    label: "Skills"
}, {
    href: "#projects",
    label: "Projects"
}, {
    href: "#experience",
    label: "Experience"
}, {
    href: "#testimonials",
    label: "Testimonials"
}]
```

### Mobile Navigation (Lines 20297-20306)

```javascript
const OR = [{
    href: "#home",
    label: "Home"
}, {
    href: "#projects",
    label: "Projects"
}, {
    href: "#contact",
    label: "Contact"
}]
```

---

## 🎯 About Section

### Mission Statement (Line 26416)

```javascript
children: "I craft game-inspired web experiences that are fast, tactile, and deliberately playful..."
```

### Core Abilities/Skills (Lines 26225-26248)

```javascript
const vN = [{
    icon: "⚡",
    name: "React & Next.js",
    level: "Expert"
}, {
    icon: "🎨",
    name: "UI/UX Design",
    level: "Advanced"
}, {
    icon: "🚀",
    name: "Performance",
    level: "Expert"
}, {
    icon: "💎",
    name: "TypeScript",
    level: "Advanced"
}, {
    icon: "🎭",
    name: "Framer Motion",
    level: "Expert"
}, {
    icon: "⚙️",
    name: "GSAP Animations",
    level: "Advanced"
}]
```

### Player Stats (Lines 26250-26263)

```javascript
const xN = [{
    to: 42,
    label: "Projects",
    color: "text-white"
}, {
    to: 5,
    label: "Years XP",
    color: "text-green-400"
}, {
    to: 128,
    label: "Videos",
    color: "text-yellow-400"
}]
```

### Profile Badge Tags (Line 26548)

```javascript
children: ["React", "GSAP", "Tailwind"].map(...)
```

---

## 💼 Projects (Lines 27170-27196)

```javascript
const sl = [{
    title: "Project One",
    desc: "Epic game-inspired landing page with GSAP animations.",
    image: SN,  // "/assets/1-CyuaMQLH.PNG"
    tags: ["React", "GSAP", "Tailwind"],
    points: [
        "Hero intro with timeline-based scene reveal.",
        "Magnetic cursor + hover sfx synced to UI.",
        "Optimized 60fps scroll-driven sections."
    ],
    url: "#"
}, {
    title: "Project Two",
    desc: "Full-stack app with real-time multiplayer features.",
    image: TN,  // "/assets/Capture-Dnj0oqZq.PNG"
    tags: ["Node", "Express", "MongoDB"],
    points: [...],
    url: "#"
}, {
    title: "Project Three",
    desc: "Pixel-art inspired UI with advanced motion design.",
    image: wN,  // "/assets/img1-BwCM-bx2.JPG"
    tags: ["Framer Motion", "Next.js", "Vite"],
    points: [...],
    url: "#"
}]
```

### Project Images (Lines 27166-27168)

```javascript
const SN = "/assets/1-CyuaMQLH.PNG"
const TN = "/assets/Capture-Dnj0oqZq.PNG"
const wN = "/assets/img1-BwCM-bx2.JPG"
```

---

## 💼 Experience/Work History (Lines 26600-26638)

```javascript
const ms = [{
    id: "neo",
    company: "NeoArcade Labs",
    role: "Senior Frontend Engineer",
    dates: "2023 — Present",
    location: "Remote",
    summary: "Motion-first rebuild (GSAP/Framer) to 60fps...",
    bullets: [
        "Onboarding timeline reduced drop-off by 18%.",
        "Headless motion primitives enabled safe animation composition.",
        "Perf budgets and CI checks improved LCP 2.8s → 1.7s."
    ],
    tags: ["React", "GSAP", "Framer Motion", "Next.js", "Tailwind", "Vite"]
}, {
    id: "code",
    company: "CodeArrays",
    role: "Full‑Stack Developer",
    dates: "2022 — 2023",
    location: "Hybrid",
    ...
}, {
    id: "hyper",
    company: "HyperPlay Studios",
    role: "Frontend Engineer",
    dates: "2020 — 2022",
    location: "On-site",
    ...
}, {
    id: "synth",
    company: "SynthOS",
    role: "UI Engineer",
    dates: "2018 — 2020",
    location: "Remote",
    ...
}]
```

---

## 💬 Testimonials (Lines 27447-27466)

```javascript
const c = [{
    quote: "Working with Gaurav was a game-changer...",
    name: "Jane Doe",
    title: "CEO, Creative Minds LLC",
    rating: 5,
    avatar: "👩‍💼"
}, {
    quote: "An incredibly talented developer...",
    name: "John Smith",
    title: "Project Manager, Tech Solutions Inc.",
    rating: 5,
    avatar: "👨‍💻"
}, {
    quote: "The passion and dedication brought to our project...",
    name: "Sam Wilson",
    title: "Lead Designer, Innovate Co.",
    rating: 5,
    avatar: "🎨"
}]
```

---

## 📧 Contact Information

### Email Address (Lines 28249-28251)

```javascript
href: "mailto:contactgaurav8@gmail.com"
children: "Contactgaurav8@gmail.com"
```

### Contact Form Email Recipient (Line 27963)

```javascript
href: "mailto:contact@example.com"
```

---

## 🖼️ Images & Assets

| Purpose           | Variable | Line  | Path                               |
|-------------------|----------|-------|------------------------------------|
| Profile (Hero)    | `kR`     | 20415 | `/assets/profile-D8-g5WhZ.png`     |
| About Photo       | `yN`     | 26223 | `/assets/about-C0vwj3CE.JPG`       |
| Project 1 Image   | `SN`     | 27166 | `/assets/1-CyuaMQLH.PNG`           |
| Project 2 Image   | `TN`     | 27167 | `/assets/Capture-Dnj0oqZq.PNG`     |
| Project 3 Image   | `wN`     | 27168 | `/assets/img1-BwCM-bx2.JPG`        |
| Contact Profile   | `DN`     | 27700 | `/assets/profile-BppvMIsH.jpg`     |
| Background Music  | `LN`     | 29046 | `/assets/game-CmnNFalC.mp3`        |

### Background Textures (Line 1446, 27820, 27826, 27832)

- `/assets/starfield-matte.png` - Starfield background
- `/assets/pixel-mountains.png` - Pixel mountain silhouette
- `/assets/frame-accents.png` - Decorative frame accents

---

## 🎵 Audio Settings (Lines 28976, 29046)

```javascript
// Background music source
const LN = "/assets/game-CmnNFalC.mp3";

// Audio component settings
{
    src: LN,
    volume: 0.5,      // Volume level (0-1)
    loop: true,       // Loop the music
    fadeMs: 800,      // Fade duration in ms
    preload: "auto"   // Preload setting
}
```

---

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

## 🛠️ Running Locally

```bash
# Start a local server
python -m http.server 8080

# Open in browser
http://localhost:8080/portfolio.html
```
