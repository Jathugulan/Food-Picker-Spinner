<div align="center">

# 🍕 Food Picker Spinner — FoodSpin

<img src="https://img.shields.io/badge/FoodSpin-Food%20Picker%20Spinner-orange?style=for-the-badge" alt="FoodSpin">

<p>
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React">
  <img src="https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Framer%20Motion-11-EF008C?style=for-the-badge" alt="Framer Motion">
  <img src="https://img.shields.io/badge/Recharts-2-22C55E?style=for-the-badge" alt="Recharts">
  <img src="https://img.shields.io/badge/Netlify-Live-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" alt="Netlify">
</p>

<p>
  <img src="https://img.shields.io/badge/License-Educational-blue?style=flat-square" alt="License">
  <img src="https://img.shields.io/badge/Status-Active-success?style=flat-square" alt="Status">
  <img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square" alt="PRs Welcome">
  <img src="https://img.shields.io/badge/Made%20with-%E2%9D%A4-red?style=flat-square" alt="Made with love">
</p>

### 🎯 Spin • Decide • Enjoy

A modern, interactive and responsive food decision-making web application that helps users quickly decide what to eat using a fun animated spinning wheel.

**🌐 [Live Demo →](https://food-picker-spinner.netlify.app)**

</div>

---

## 📑 Table of Contents

- [About FoodSpin](#-about-foodspin)
- [Key Features](#-key-features)
- [Screenshots](#️-screenshot-gallery)
- [Application Pages](#-application-pages)
- [Technology Stack](#-technology-stack)
- [System Architecture](#️-system-architecture)
- [Project Structure](#-project-structure)
- [Spinner Algorithm](#-spinner-algorithm)
- [Getting Started](#-getting-started)
- [Available Scripts](#-available-scripts)
- [Deployment](#-netlify-deployment)
- [Keyboard Shortcuts](#-keyboard-shortcuts)
- [Accessibility](#-accessibility)
- [Data & Privacy](#-data--privacy)
- [Testing & Validation](#-testing--validation)
- [Performance](#-performance)
- [Roadmap](#-roadmap--future-enhancements)
- [FAQ](#-faq)
- [Contributing](#-contributing)
- [Issues & Feedback](#-issues--feedback)
- [License](#-license)
- [Author](#-author)

---

## 📖 About FoodSpin

**Food Picker Spinner (FoodSpin)** is a modern Single Page Application built to solve the everyday problem of:

> **"What should I eat today?" 🍕🍔🍜**

Instead of endlessly scrolling menus or debating with friends, users can manage a personal food collection, organize it into categories, spin an interactive wheel, review past results, and analyze their own food-selection habits through visual statistics.

FoodSpin runs entirely client-side, persisting data through the browser's `localStorage` — no backend server, database, or account is required to use the core app.

---

## ✨ Key Features

### 🎡 1. Interactive Food Spinner

The centerpiece of FoodSpin — a fully animated decision wheel.

| Feature | Description |
|---|---|
| 🎡 Animated wheel | Smooth, physics-like spin animation |
| 🍕 Dynamic segments | Wheel auto-divides based on active food count |
| 🎲 Random selection | Fair, unbiased food picking |
| 🌀 Realistic motion | Acceleration → deceleration → settle |
| 🎯 Pointer accuracy | Winner always aligns precisely with the pointer |
| 🏆 Result reveal | Animated winner callout with confetti-style feedback |
| 🎯 Category filters | Spin within a specific category only |
| 👆 Touch-friendly | Optimized for tap-to-spin on mobile |
| ♻️ Re-spin / exclude | Optionally exclude the last winner from the next spin |

```text
Segment Angle = 360° / N   (N = number of active food items)
```

### 🍔 2. Food Management (CRUD)

- ➕ Add, ✏️ edit, 🗑️ delete food items
- ❤️ Mark favorites · ⭐ Rate items · 🏷️ Tag items
- 📝 Add descriptions and 📂 assign categories
- 🔍 Search & filter your food list
- 🎯 Toggle items in/out of the active spinner pool
- 🖼️ Emoji-based food icons (no image uploads required)

**Food entity schema:**

```text
{
  id, name, category, emoji,
  description, favorite, rating, tag
}
```

### 📂 3. Category Management

- ➕✏️🗑️ Full CRUD for categories
- 🍔 Group and filter foods by category
- 📊 Per-category selection statistics
- 🎯 Category-scoped spins

```text
🍕 Pizza  🍔 Burgers  🍜 Asian  🍛 Rice  🥗 Healthy  🍰 Desserts  🥤 Drinks
```

### 🕘 4. Spin History

- 🕘 Chronological log of every spin result
- 📅 Timestamped entries
- 🔍 Review and revisit past decisions
- 🗑️ Clear history (single entry or full wipe)
- 💾 Persists across page refreshes via `localStorage`

### 📊 5. Statistics Dashboard

- 📈 Selection frequency per food
- 🏆 "Most picked" leaderboard
- 📂 Category-level breakdowns
- 📉 Historical trend visualization
- 🔢 Total spin counter
- 📊 Interactive charts powered by **Recharts**

### 🏠 6. Home Dashboard

- 🎯 One-tap "Quick Spin"
- 🍕 Food & 📂 category overview widgets
- 🕘 Recent history preview
- 📊 Statistics snapshot
- ❤️ Favorites shortcut
- ✨ Animated widgets on load

### 🌙 7. Theme Support

- ☀️ Light · 🌙 Dark · 🖥️ System/Auto
- Custom Tailwind design tokens for backgrounds, cards, gradients & accents
- Instant, flicker-free theme switching

### 📱 8. Fully Responsive Design

| Device | Support |
|---|---|
| 📱 Mobile | ✅ |
| 📱 Large Mobile | ✅ |
| 📲 Tablet | ✅ |
| 💻 Laptop | ✅ |
| 🖥️ Desktop | ✅ |
| 🖥️ Large Desktop | ✅ |

Mobile-first layouts, responsive nav, adaptive spinner sizing, flexible grids, and zero unwanted horizontal scroll.

### 💾 9. LocalStorage Persistence

No backend needed for core functionality.

```text
foodspin_foods
foodspin_categories
foodspin_history
foodspin_settings
```

### ⚡ 10. Performance Optimization

Vite production builds, optimized static assets, component-level code structure, efficient Tailwind purging, and lightweight client-side rendering.

### 🎨 11. Premium UI/UX

Modern cards, gradient accents, glass-style surfaces, consistent spacing system, micro-interactions, and intuitive navigation throughout.

### 🆕 12. New in This Update

- 🔔 **Toast notifications** for add/edit/delete actions
- ⌨️ **Keyboard shortcuts** for power users (spin, search, theme toggle)
- 📤 **Export / Import** food data as JSON for backup or sharing
- 🧩 **Empty states** with helpful guidance when lists are empty
- 🎚️ **Spin speed control** (slow / normal / fast)
- 🔍 **Global search** across foods and categories
- ♿ **Improved accessibility** — focus states, ARIA labels, reduced-motion support
- 🧭 **Breadcrumb navigation** on nested views

---

## 🖼️ Screenshot Gallery

| Home | Spinner |
|---|---|
| ![Home](screenshots/home.jpg) | ![Spinner](screenshots/spinner.jpg) |

| Foods | Categories |
|---|---|
| ![Foods](screenshots/foods.jpg) | ![Categories](screenshots/categories.jpg) |

| Statistics | History |
|---|---|
| ![Statistics](screenshots/statistics.jpg) | ![History](screenshots/history.jpg) |

---

## 🧭 Application Pages

| Page | Description | Screenshot |
|---|---|---|
| 🏠 Home | Application dashboard & quick actions | `screenshots/home.jpg` |
| 🎡 Spinner | Interactive food picker wheel | `screenshots/spinner.jpg` |
| 🍔 Foods | Manage food items (CRUD) | `screenshots/foods.jpg` |
| 📂 Categories | Manage food categories | `screenshots/categories.jpg` |
| 📊 Statistics | Selection analytics & charts | `screenshots/statistics.jpg` |
| 🕘 History | Log of previous spins | `screenshots/history.jpg` |
| ⚙️ Settings | Theme, data export/import, preferences | — |

---

## 🧰 Technology Stack

### 🎨 Frontend

<p>
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React 19">
  <img src="https://img.shields.io/badge/Vite-5-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite 5">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS 3">
  <img src="https://img.shields.io/badge/Framer%20Motion-11-EF008C?style=flat-square&logo=framer&logoColor=white" alt="Framer Motion 11">
  <img src="https://img.shields.io/badge/Recharts-2-22C55E?style=flat-square" alt="Recharts 2">
  <img src="https://img.shields.io/badge/React%20Router-DOM-CA4245?style=flat-square&logo=reactrouter&logoColor=white" alt="React Router">
  <img src="https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript ES6+">
</p>

### 🌐 Browser Technologies

<p>
  <img src="https://img.shields.io/badge/localStorage-Web%20Storage%20API-4B5563?style=flat-square" alt="localStorage">
  <img src="https://img.shields.io/badge/SVG-Vector%20Graphics-FFB13B?style=flat-square&logo=svg&logoColor=black" alt="SVG">
  <img src="https://img.shields.io/badge/Web%20Storage%20API-Client%20Side-6366F1?style=flat-square" alt="Web Storage API">
</p>

### 🛠️ Dev Tooling

<p>
  <img src="https://img.shields.io/badge/ESLint-Linting-4B32C3?style=flat-square&logo=eslint&logoColor=white" alt="ESLint">
  <img src="https://img.shields.io/badge/PostCSS-CSS%20Processing-DD3A0A?style=flat-square&logo=postcss&logoColor=white" alt="PostCSS">
  <img src="https://img.shields.io/badge/npm-Package%20Manager-CB3837?style=flat-square&logo=npm&logoColor=white" alt="npm">
</p>

### 🚀 Deployment

<p>
  <img src="https://img.shields.io/badge/GitHub-Version%20Control-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub">
  <img src="https://img.shields.io/badge/Netlify-Hosting-00C7B7?style=flat-square&logo=netlify&logoColor=white" alt="Netlify">
</p>

### 📊 Stack at a Glance

| Layer | Technology | Purpose |
|---|---|---|
| ⚛️ UI Library | React 19 | Component-based interface |
| ⚡ Build Tool | Vite 5 | Fast dev server & bundling |
| 🎨 Styling | Tailwind CSS 3 | Utility-first responsive design |
| 🌀 Animation | Framer Motion | Spinner & UI motion effects |
| 📈 Charts | Recharts 2 | Statistics dashboard visuals |
| 🧭 Routing | React Router | SPA page navigation |
| 💾 Persistence | localStorage | Client-side data storage |
| 🔍 Linting | ESLint | Code quality & consistency |
| ☁️ Hosting | Netlify | Continuous deployment from GitHub |

---

## 🏗️ System Architecture

```text
                    ┌─────────────────────┐
                    │      FoodSpin       │
                    │      React SPA      │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
        ┌─────────┐      ┌───────────┐     ┌─────────┐
        │  Pages  │      │ Components│     │ Router  │
        └────┬────┘      └─────┬─────┘     └─────────┘
             │                 │
             └────────┬────────┘
                       ▼
              ┌────────────────┐
              │  Custom Hooks  │
              │ useLocalStorage│
              └────────┬───────┘
                       │
                       ▼
              ┌────────────────┐
              │  localStorage  │
              └────────────────┘
```

---

## 📁 Project Structure

```text
FoodSpin/
│
├── public/
│
├── screenshots/
│   ├── home.jpg
│   ├── categories.jpg
│   ├── history.jpg
│   ├── statistics.jpg
│   ├── foods.jpg
│   └── spinner.jpg
│
├── src/
│   ├── components/
│   │   ├── SpinnerWheel.jsx
│   │   ├── Navbar.jsx
│   │   ├── ThemeToggle.jsx
│   │   └── Toast.jsx
│   │
│   ├── hooks/
│   │   ├── useLocalStorage.js
│   │   └── useTheme.js
│   │
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── Spinner.jsx
│   │   ├── Foods.jsx
│   │   ├── Categories.jsx
│   │   ├── Statistics.jsx
│   │   ├── History.jsx
│   │   └── Settings.jsx
│   │
│   ├── utils/
│   │   ├── spinnerUtils.js
│   │   └── exportImport.js
│   │
│   ├── App.jsx
│   └── main.jsx
│
├── package.json
├── tailwind.config.js
├── vite.config.js
└── README.md
```

---

## 🧮 Spinner Algorithm

FoodSpin dynamically divides the wheel into equal segments for `N` active food items:

```text
θ = 360° / N
```

For each segment, the app calculates:

```text
Start Angle
End Angle
Center Angle
Target Rotation
```

A random target segment is chosen, then the wheel spins through several full rotations before decelerating and settling so the winning segment aligns exactly with the pointer — powered by **Framer Motion** easing curves for a natural, physical feel.

---

## 🚀 Getting Started

### Prerequisites

```text
Node.js 18+
npm 9+
```

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

### 2. Enter the project folder

```bash
cd FoodSpin
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

Open the local URL Vite prints in your terminal (typically `http://localhost:5173`).

---

## 📜 Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start the local development server with hot reload |
| `npm run build` | Create an optimized production build in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run ESLint across the codebase |

---

## 🚀 Netlify Deployment

### Build Configuration

```text
Branch:              main
Build command:       npm run build
Publish directory:   dist
Base directory:      (empty)
Functions directory: (empty)
```

### 🔄 Deployment Workflow

```text
Developer → GitHub Repository → Push to main
    → Netlify Build → npm run build → dist/
    → Netlify CDN → 🌐 Live FoodSpin Website
```

**🌐 Live Site:** https://food-picker-spinner.netlify.app

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Space` | Spin the wheel |
| `/` | Focus the search bar |
| `T` | Toggle light/dark theme |
| `Esc` | Close open modal/dialog |

---

## ♿ Accessibility

- Semantic HTML structure across pages
- Visible focus states on all interactive elements
- ARIA labels on icon-only buttons
- Sufficient color contrast in both light and dark themes
- `prefers-reduced-motion` support for the spinner animation

---

## 🔐 Data & Privacy

FoodSpin is a fully client-side application:

- Food data, categories, and spin history are stored **only** in your browser's `localStorage`
- No backend server, account, or tracking is required for core functionality
- Use **Export** in Settings to back up your data as a JSON file
- Use **Import** to restore or transfer data to another browser/device
- Clearing your browser storage will permanently remove locally saved data

---

## 🧪 Testing & Validation

### Responsive Viewports Tested

| Device | Resolution |
|---|---|
| 🖥️ Desktop | 1280 × 850 |
| 📲 Tablet | 768 × 1024 |
| 📱 Mobile | 375 × 812 |

### Validation Checklist

- ✅ Production build
- ✅ Page navigation
- ✅ Spinner functionality & accuracy
- ✅ Food CRUD operations
- ✅ Category management
- ✅ History persistence
- ✅ Statistics accuracy
- ✅ Theme switching
- ✅ Responsive layouts
- ✅ Mobile navigation
- ✅ Browser refresh behavior
- ✅ Data export/import round-trip

---

## 📈 Performance

```text
Total Build Package: 494.96 kB
Gzip Size:            139.80 kB

Performance Score:    98/100
FCP:                  0.4s
LCP:                  0.8s
CLS:                  0.00
TBT:                  0ms
```

> Performance results may vary depending on browser, device, network, and deployment conditions.

---

## 🎯 Project Goals

- 🍕 Reduce everyday food decision fatigue
- 🎡 Make food selection fun and engaging
- 🍔 Provide a simple, effective food-management system
- 📂 Help users organize choices by category
- 📊 Surface useful selection statistics
- 🕘 Maintain a reliable spin history
- 📱 Deliver a fast, responsive, modern UI
- ⚡ Stay lightweight with zero backend dependency

---

## 🗺️ Roadmap / Future Enhancements

- 🤖 AI-powered food recommendations
- 🌦️ Weather-based food suggestions
- 📍 Location-based restaurant recommendations
- 🥗 Nutrition information per food item
- 🔐 Optional user authentication
- ☁️ Cloud sync across devices
- 📱 PWA support (installable, offline-capable)
- 🔔 Reminder notifications ("Time to decide dinner!")
- 🎵 Spinner sound effects
- 🌎 Multi-language support (i18n)
- 📊 Advanced analytics (streaks, trends over time)
- 👥 Shared/collaborative food lists
- 🎨 Custom, user-created spinner themes

---

## ❓ FAQ

**Does FoodSpin need an internet connection?**
No — after the initial page load, the app runs entirely offline using `localStorage`.

**Will I lose my data if I clear my browser cache?**
Yes, since data lives in `localStorage`. Use the Export feature in Settings to back it up first.

**Can I use FoodSpin on my phone?**
Yes, the entire UI — including the spinner — is fully responsive and touch-optimized.

**Is there a backend or database?**
No. FoodSpin is a pure client-side SPA by design, which keeps it fast and privacy-friendly.

---

## 🏆 Project Highlights

```text
✨ Premium Modern UI
🎡 Interactive Food Spinner
🍔 Complete Food Management
📂 Category Management
🕘 Spin History
📊 Statistics Dashboard
🏠 Home Dashboard
🌙 Theme Support
📱 Fully Responsive
💾 LocalStorage Persistence
📤 Data Export/Import
♿ Accessibility Enhancements
⚡ Vite Performance
🌀 Framer Motion Animations
📈 Recharts Analytics
🚀 Netlify Deployment
🔒 Client-Side Privacy
```

---

## 🤝 Contributing

Contributions are welcome!

```bash
# 1. Fork the repository

# 2. Create a feature branch
git checkout -b feature/new-feature

# 3. Commit your changes
git add .
git commit -m "feat: add new feature"

# 4. Push the branch
git push origin feature/new-feature
```

Then open a Pull Request describing your changes.

---

## 🐛 Issues & Feedback

If you discover a bug or have a suggestion:

1. Open a GitHub Issue
2. Describe the problem clearly
3. Include reproduction steps
4. Attach screenshots when useful
5. Suggest an improvement if possible

---

## 📄 License

This project is intended for educational and portfolio purposes.

---

## 👨‍💻 Author

### Raveendran Jathugulan

**Full-Stack Developer | MERN Stack Developer | BICT Undergraduate**

Passionate about building modern, responsive, and user-friendly web applications.

**🌐 Connect**

* 🐙 GitHub: [Jathugulan](https://github.com/Jathugulan)
* 💼 LinkedIn: [Raveendran Jathugulan](https://www.linkedin.com/in/raveendran-jathugulan/)
* 🌐 Live Project: [FoodSpin](https://food-picker-spinner.netlify.app)

---

## ⭐ Support

If you like **FoodSpin**, please consider giving the repository a ⭐ on GitHub — it helps a lot!

<div align="center">

### 🍕 Spin Your Way to Your Next Meal! 🎡

**Made with ❤️ using React, Vite & Tailwind CSS**

</div>
