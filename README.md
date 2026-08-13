<div align="center">

# 🍕 Food Picker Spinner (FoodSpin)

[![React](https://img.shields.io/badge/React-19.0.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-5.4.1-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4.4-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-11.0.0-E10098?style=for-the-badge&logo=framer&logoColor=white)](https://www.framer.com/motion/)
[![Recharts](https://img.shields.io/badge/Recharts-2.8.0-22C55E?style=for-the-badge&logo=chart.js&logoColor=white)](https://recharts.org/)
[![Netlify](https://img.shields.io/badge/Netlify-Live-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)](https://food-picker-spinner.netlify.app)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

### 🎯 Spin • Decide • Enjoy

**FoodSpin** is a modern, responsive, and feature-packed web app built to eliminate decision fatigue around dining. Powered by **React 19**, **Vite 5**, **Tailwind CSS**, and **Framer Motion**, it turns meal selection into an interactive, gamified experience — complete with physics-inspired spinning animations, custom menu management, visual statistics, spin logs, and local-first data privacy.

**🌐 [Live Demo →](https://food-picker-spinner.netlify.app)**

</div>

---

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Features](#-features)
- [Screenshots](#️-screenshots)
- [Technologies Used](#️-technologies-used)
- [Installation & Local Setup](#-installation--local-setup)
- [Available Scripts](#-available-scripts)
- [Usage Guide](#-usage-guide)
- [Project Architecture](#️-project-architecture)
- [Deployment](#-deployment-instructions)
- [License](#️-license)

---

## 📌 Project Overview

Have you ever wasted 30 minutes asking, *"What should we eat today?"*

**FoodSpin** solves the classic "where should we eat" dilemma. Whether deciding between pizza, sushi, tacos, or home-cooked meals, it lets you spin a dynamic SVG wheel, filter by custom culinary categories, track spin analytics over time, and keep a log of past choices.

### Key Highlights

- 🧠 **Eliminates Choice Paralysis** — takes the stress out of daily meal decisions
- ⚡ **Lightning Fast & Responsive** — built with Vite and React 19 for instant interactions
- 🔒 **100% Client-Side Privacy** — foods, categories, settings, and history are persisted locally in `localStorage`, no server or tracking required
- 🎨 **Modern Aesthetics** — sleek dark/light themes with glassmorphism UI and micro-animations

---

## ✨ Features

### 🎡 Interactive SVG Spinner Wheel

- **Physics-inspired deceleration** using a `cubic-bezier(0.15, 0.85, 0.35, 1.0)` easing curve for a realistic, smooth stop
- **Dynamic arc calculations** — trigonometric SVG geometry recalculates slice angles, labels, and gradients based on active food selections
- **Smart pointer alignment** — precise angle-to-item mapping lands the winner exactly under the pointer needle
- **Winner celebration modal** with confetti animation, plus options to save to history, spin again, or exclude the chosen meal

### 🍱 Food & Menu Management

- Full **CRUD** — add, edit, search, and delete meal options
- **Custom emojis & tagging** (e.g. Spicy, Vegan, Fast Food, Healthy)
- **Favorites system** for quick-toggle filtering or dedicated spins

### 🏷️ Custom Categories Manager

- Group foods into custom categories — *Italian*, *Asian*, *Fast Food*, *Desserts*, *Breakfast*, and more
- Live counters showing how many dishes belong to each category

### 📊 Analytics & Statistics Dashboard

- **Recharts**-powered bar graphs of most-chosen items and category distribution pie charts
- Spin trend insights into your dining habits and cravings

### 📜 Historical Audit Log

- Chronological spin logs with timestamps and category badges
- Remove individual entries or clear the full history in one click

### ⚙️ User Customization & Data Governance

- **Theme support** — Light, Dark, and Auto (system-aware)
- **Spin duration control** — configurable from 3s to 10s
- **Avoid recently picked items** — smart toggle to exclude recent winners from upcoming spins
- **Backup & restore** — export full app state (foods, categories, history, settings) to a JSON file and import it anytime

---

## 🖼️ Screenshots

<div align="center">

### 🏠 Home Dashboard
*Quick access to the spinner, menu overview, statistics, and category highlights.*

![Home Screen](./screenshots/home.png)

---

### 🎡 Interactive Spinner Wheel
*Dynamic SVG wheel with category filters, physics-based rotation, and a confetti winner modal.*

![Spinner](./screenshots/spinner.png)

---

### 🍱 Food Items Management
*Browse, filter, search, and manage every food choice.*

![Foods](./screenshots/foods.png)

---

### 🏷️ Categories Manager
*Organize dishes into custom culinary categories with live item counts.*

![Categories](./screenshots/categories.png)

---

### 📜 Decision History
*Timestamped audit trail of past spin results.*

![History](./screenshots/history.png)

---

### 📊 Analytics & Statistics
*Charts illustrating choice counts, category distribution, and top picks.*

![Statistics](./screenshots/statistics.png)

</div>

> 📁 Screenshots live in the [`/screenshots`](./screenshots) folder at the project root. Make sure the file names above (`home.png`, `spinner.png`, `foods.png`, `categories.png`, `history.png`, `statistics.png`) match exactly (case-sensitive) so they render correctly on GitHub.

---

## 🛠️ Technologies Used

| Layer / Aspect | Technology | Version | Purpose |
| :--- | :--- | :--- | :--- |
| **Frontend Framework** | [React](https://react.dev/) | `^19.0.0` | UI component lifecycle, hooks-driven state architecture |
| **Build Tooling & Dev Server** | [Vite](https://vitejs.dev/) | `^5.4.1` | Next-generation ESM bundler with ultra-fast HMR |
| **Styling & Design System** | [Tailwind CSS](https://tailwindcss.com/) | `^3.4.4` | Utility-first CSS with custom glassmorphism design tokens |
| **Animation Engine** | [Framer Motion](https://www.framer.com/motion/) | `^11.0.0` | Declarative SVG rotation, modal transitions, list animations |
| **Data Visualization** | [Recharts](https://recharts.org/) | `^2.8.0` | SVG-based responsive analytics charts (BarChart, PieChart) |
| **Routing** | [React Router](https://reactrouter.com/) | `^6.18.0` | SPA client-side route management |
| **Icons** | [Lucide React](https://lucide.dev/) | `^0.499.0` | Scalable modern icon set |
| **Data Persistence** | HTML5 `localStorage` API | Native | Client-side storage via a custom `useLocalStorage` hook |

---

## 🚀 Installation & Local Setup

### Prerequisites

- **Node.js** `v18.0.0` or higher — [Download Node.js](https://nodejs.org/)
- **Package manager** — `npm` (comes with Node.js), or `yarn` / `pnpm`

### Step-by-Step

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/food-picker-spinner.git
   cd food-picker-spinner
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Open in your browser**
   Navigate to `http://localhost:5173` to explore the app.

---

## 📜 Available Scripts

| Command | Action |
| :--- | :--- |
| `npm run dev` | Starts the Vite dev server with Hot Module Replacement (HMR) |
| `npm run build` | Compiles and optimizes production assets into `/dist` |
| `npm run preview` | Serves the built production bundle locally for preview |

---

## 🎯 Usage Guide

1. **Spin for a decision**
   - Open the **Spinner** page from the navigation
   - Choose a category filter (*Fast Food*, *Asian*, *All Foods*, etc.)
   - Click **"SPIN THE WHEEL"**
   - When it lands, a celebration modal opens — **Save to History** or **Spin Again**

2. **Add custom foods**
   - Go to the **Foods** page → **"+ Add Food"**
   - Enter a name, pick a category and emoji, add optional tags/favorite
   - Click **"Save Food"**

3. **Manage categories**
   - Go to **Categories** to create custom groups (e.g. *Late Night Snacks*)
   - Edit or delete existing categories anytime

4. **View stats & history**
   - **Statistics** — visual charts on your dining habits
   - **History** — timestamped record of every spin

5. **Backup & export data**
   - Go to **Settings → Data Management**
   - **Export Data** downloads a `.json` snapshot of your app state
   - **Import Data** restores from a previously saved file

---

## 🏗️ Project Architecture

```text
FoodSpin/
├── screenshots/                # README screenshot assets
│   ├── home.png
│   ├── spinner.png
│   ├── foods.png
│   ├── categories.png
│   ├── history.png
│   └── statistics.png
│
├── public/
│   └── favicon.svg
│
├── src/
│   ├── components/              # Reusable UI components
│   │   ├── CategoryFilter.jsx
│   │   ├── Confetti.jsx
│   │   ├── FoodCard.jsx
│   │   ├── FoodForm.jsx
│   │   ├── Navbar.jsx
│   │   ├── SpinnerWheel.jsx
│   │   ├── Toast.jsx
│   │   └── WinnerModal.jsx
│   │
│   ├── data/
│   │   └── defaultFoods.js      # Default starter food items & categories
│   │
│   ├── hooks/
│   │   └── useLocalStorage.js   # Custom hook for localStorage persistence
│   │
│   ├── pages/                   # Top-level route views
│   │   ├── Categories.jsx
│   │   ├── Foods.jsx
│   │   ├── History.jsx
│   │   ├── Home.jsx
│   │   ├── Settings.jsx
│   │   ├── Spinner.jsx
│   │   └── Statistics.jsx
│   │
│   ├── utils/
│   │   └── spinnerUtils.js      # Trigonometric wheel calculations & SVG math
│   │
│   ├── App.jsx                  # App shell, routing, theme provider
│   ├── index.css                # Tailwind directives & custom styles
│   └── main.jsx                 # React DOM root mounting script
│
├── index.html
├── package.json
├── postcss.config.js
├── tailwind.config.js
└── vite.config.js
```

---

## 🌐 Deployment Instructions

### ✅ Live Deployment (Netlify)

FoodSpin is currently deployed and live at:

**🔗 https://food-picker-spinner.netlify.app**

**Build configuration used:**

```text
Build command:       npm run build
Publish directory:   dist
Base directory:      (empty)
Functions directory: (empty)
```

### Deploy Your Own

<details>
<summary><strong>Option 1: Netlify</strong></summary>

1. Sign in to [Netlify](https://www.netlify.com/) → **"Add new site" → "Import an existing project"**
2. Connect your GitHub repository
3. Configure build settings:
   - **Build Command:** `npm run build`
   - **Publish Directory:** `dist`
4. For client-side routing support, add a `public/_redirects` file with:
   ```text
   /*   /index.html   200
   ```
5. Click **Deploy Site**

</details>

<details>
<summary><strong>Option 2: Vercel</strong></summary>

1. Push your project code to GitHub
2. Sign in to [Vercel](https://vercel.com/) → **"Add New Project"**
3. Import your GitHub repository
4. Vercel auto-detects Vite:
   - **Framework Preset:** Vite
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
5. Click **Deploy**

</details>

<details>
<summary><strong>Option 3: GitHub Pages</strong></summary>

1. Update `vite.config.js` to set the `base` path:
   ```javascript
   export default defineConfig({
     base: '/food-picker-spinner/',
     plugins: [react()],
   })
   ```
2. Build the static bundle:
   ```bash
   npm run build
   ```
3. Deploy the contents of `dist/` to your repository's `gh-pages` branch

</details>

<details>
<summary><strong>Option 4: Docker & Nginx</strong></summary>

**`Dockerfile`:**

```dockerfile
# Stage 1: Build production bundle
FROM node:18-alpine AS build
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build

# Stage 2: Serve with Nginx
FROM nginx:alpine
COPY --from=build /app/dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

Build and run:

```bash
docker build -t food-picker-spinner .
docker run -p 8080:80 food-picker-spinner
```

</details>

---

## ⚖️ License

This project is licensed under the **MIT License**. See the [`LICENSE`](LICENSE) file for details.

---

<div align="center">

### 🍕 Spin Your Way to Your Next Meal! 🎡

Made with ❤️ for food lovers and indecisive eaters everywhere.

**🌐 [Live Demo](https://food-picker-spinner.netlify.app) · 🐙 [GitHub](https://github.com/Jathugulan)**

</div>