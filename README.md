# 🍕 Food Picker Spinner (FoodSpin)

[![React](https://img.shields.io/badge/React-19.0.0-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-5.4.1-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.4.4-38BDF8?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer_Motion-11.0.0-E10098?style=for-the-badge&logo=framer&logoColor=white)](https://www.framer.com/motion/)
[![Recharts](https://img.shields.io/badge/Recharts-2.8.0-22C55E?style=for-the-badge&logo=chart.js&logoColor=white)](https://recharts.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

**Food Picker Spinner (FoodSpin)** is a modern, responsive, and feature-packed web application built to eliminate decision fatigue around dining. Powered by **React 19**, **Vite 5**, **Tailwind CSS**, and **Framer Motion**, FoodSpin turns meal selection into an interactive, gamified experience complete with physics-inspired spinning animations, custom menu management, visual statistics, spin logs, and local-first data privacy.

---

## 📌 Project Overview

Have you ever wasted 30 minutes asking, *"What should we eat today?"*

**Food Picker Spinner** solves the classic "where should we eat" dilemma. Whether deciding between pizza, sushi, tacos, or home-cooked meals, FoodSpin lets users spin a dynamic SVG wheel, filter by customized culinary categories, track spin analytics over time, and keep a log of past choices.

### Key Highlights
- 🧠 **Eliminates Choice Paralysis**: Takes the stress out of daily meal decisions.
- ⚡ **Lightning Fast & Responsive**: Built with Vite and React 19 for instant interactions.
- 🔒 **100% Client-Side Privacy**: All custom items, categories, settings, and logs are persisted locally in `localStorage` without tracking or server backend requirements.
- 🎨 **Modern Aesthetics**: Sleek dark/light themes with smooth glassmorphism UI elements and micro-animations.

---

## ✨ Features

### 🎡 Interactive SVG Spinner Wheel
- **Physics-Inspired Deceleration**: Easing algorithm with `cubic-bezier(0.15, 0.85, 0.35, 1.0)` physics curve for a realistic, smooth stop.
- **Dynamic Arc Calculations**: Trigonometric SVG geometry automatically recalculates slice angles, labels, and vibrant gradient themes based on active food selections.
- **Smart Pointer Alignment**: Precise angle-to-item mapping calculates the winner right under the pointer needle.
- **Winner Celebration Modal**: Confetti animation popups celebrate every outcome with options to save decision log, re-spin, or filter out chosen meals.

### 🍱 Food & Menu Management
- **Full CRUD Functionality**: Easily add, edit, search, and delete meal options.
- **Custom Emojis & Tagging**: Assign emojis and tags (e.g., Spicy, Vegan, Fast Food, Healthy) to each dish.
- **Favorites System**: Quick-toggle favorite meals for instant filtering or dedicated spinning.

### 🏷️ Custom Categories Manager
- **Dynamic Categorization**: Group foods into customizable categories like *Italian*, *Asian*, *Fast Food*, *Desserts*, or *Breakfast*.
- **Live Counter & Filtering**: Instant visual counters showing how many dishes belong to each category.

### 📊 Analytics & Statistical Dashboard
- **Recharts Integration**: Interactive bar graphs showcasing most-chosen food items, category distribution pie charts, and total decision metrics.
- **Spin Trends**: Gain insights into your dining habits and most frequent cravings.

### 📜 Historical Audit Log
- **Chronological Spin Logs**: View previous spin outcomes complete with timestamps and category badges.
- **Log Control**: Remove individual entries or clear spin history with one click.

### ⚙️ User Customization & Data Governance
- **Theme Support**: Seamless Light, Dark, and Auto System-aware themes.
- **Spin Duration Tweaks**: Configurable wheel spin duration (3s to 10s).
- **Avoid Recently Picked Items**: Smart toggle to exclude recently won items from upcoming spins.
- **Backup & Restore**: Export all app state (foods, categories, history, settings) to a JSON file and restore anytime.

---

## 🛠️ Technologies Used

| Layer / Aspect | Technology | Version | Purpose |
| :--- | :--- | :--- | :--- |
| **Frontend Framework** | [React](https://react.dev/) | `^19.0.0` | UI component lifecycle, hooks-driven state architecture |
| **Build Tooling & Dev Server** | [Vite](https://vitejs.dev/) | `^5.4.1` | Next-generation ESM bundler and ultra-fast HMR dev server |
| **Styling & Design System** | [Tailwind CSS](https://tailwindcss.com/) | `^3.4.4` | Utility-first CSS framework with custom glassmorphism design tokens |
| **Animation Engine** | [Framer Motion](https://www.framer.com/motion/) | `^11.0.0` | Declarative SVG rotation, modal drop-ins, and list transitions |
| **Data Visualization** | [Recharts](https://recharts.org/) | `^2.8.0` | SVG-based responsive analytics charts (BarChart, PieChart) |
| **Routing System** | [React Router](https://reactrouter.com/) | `^6.18.0` | SPA client-side route management |
| **Icons** | [Lucide React](https://lucide.dev/) | `^0.499.0` | Scalable modern icon set |
| **Data Persistence** | HTML5 `localStorage` API | Native | Client-side persistent key-value storage hook (`useLocalStorage`) |

---

## 📸 Screenshots

Here is a visual preview of the main interfaces in Food Picker Spinner:

### 🏠 Home Dashboard
*Comprehensive dashboard providing quick access to spinner, menu overview, statistics, and category highlights.*
![Home Dashboard](screenshots/home.png)

---

### 🎡 Interactive Spinner Wheel
*Dynamic SVG wheel with customizable category filters, physics rotation, and confetti winner celebration modal.*
![Interactive Spinner Wheel](screenshots/spinner.png)

---

### 🍱 Food Items Management
*Grid view for browsing, filtering, searching, and managing all food choices.*
![Food Items Grid](screenshots/foods.png)

---

### 🏷️ Categories Manager
*Organize dishes into custom culinary categories with live item counting.*
![Categories Manager](screenshots/categories.png)

---

### 📊 Analytics & Statistics
*Detailed charts illustrating choice counts, category distribution, and top picks.*
![Statistics Dashboard](screenshots/statistics.png)

---

### 📜 Decision History
*Timestamped audit trail of past spin results with filter and clear capabilities.*
![Spin History](screenshots/history.png)

---

## 🚀 Installation & Local Setup

Follow these steps to run Food Picker Spinner locally on your machine:

### Prerequisites
- **Node.js**: `v18.0.0` or higher ([Download Node.js](https://nodejs.org/))
- **Package Manager**: `npm` (comes with Node.js) or `yarn` / `pnpm`

### Step-by-Step Instructions

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/food-picker-spinner.git
   cd food-picker-spinner
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Start Development Server**
   ```bash
   npm run dev
   ```

4. **Open in Browser**
   Open your browser and navigate to `http://localhost:5173` to explore the application.

---

## 📜 Available Scripts

In the root directory, you can execute the following commands:

| Command | Action |
| :--- | :--- |
| `npm run dev` | Starts Vite local development server with Hot Module Replacement (HMR). |
| `npm run build` | Compiles and optimizes production assets into the `/dist` directory. |
| `npm run preview` | Spins up a local static server to preview the built production bundle. |

---

## 🎯 Usage Guide

1. **Spinning for a Decision**:
   - Go to **Spinner** page from top or mobile navigation.
   - Choose a category filter (e.g., *Fast Food*, *Asian*, or *All Foods*).
   - Click **"SPIN THE WHEEL"**.
   - When the wheel lands on a meal, a celebration modal opens. Click **"Save to History"** or **"Spin Again"**.

2. **Adding Custom Foods**:
   - Navigate to **Foods** page.
   - Click **"+ Add Food"**.
   - Enter food name, select category, pick an emoji, and add optional tags/favorites.
   - Click **"Save Food"**.

3. **Managing Categories**:
   - Go to **Categories** page to create custom categories (e.g. *Late Night Snacks*).
   - Edit or delete existing categories as needed.

4. **Viewing Stats & History**:
   - Check **Statistics** to see visual charts on your dining habits.
   - Check **History** for timestamped records of all spins.

5. **Backup & Data Export**:
   - Navigate to **Settings** -> **Data Management**.
   - Click **"Export Data"** to download a `.json` snapshot of your current app data.
   - Click **"Import Data"** to restore from a previously saved file.

---

## 🏗️ Project Architecture

```
Food Picker Spinner/
├── public/                  # Static assets & app favicon
│   ├── favicon.svg
│   └── screenshots/         # Application visual previews
├── screenshots/             # Repository documentation screenshots
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── CategoryFilter.jsx
│   │   ├── Confetti.jsx
│   │   ├── FoodCard.jsx
│   │   ├── FoodForm.jsx
│   │   ├── Navbar.jsx
│   │   ├── SpinnerWheel.jsx
│   │   ├── Toast.jsx
│   │   └── WinnerModal.jsx
│   ├── data/
│   │   └── defaultFoods.js  # Default starter food items & categories
│   ├── hooks/
│   │   └── useLocalStorage.js # Custom hook for HTML5 LocalStorage persistence
│   ├── pages/               # React Router top-level view pages
│   │   ├── Categories.jsx
│   │   ├── Foods.jsx
│   │   ├── History.jsx
│   │   ├── Home.jsx
│   │   ├── Settings.jsx
│   │   ├── Spinner.jsx
│   │   └── Statistics.jsx
│   ├── utils/
│   │   └── spinnerUtils.js  # Trigonometric wheel calculations & SVG math
│   ├── App.jsx              # Application root shell, routing, & theme provider
│   ├── index.css            # Tailwind directives, custom fonts, glassmorphism styles
│   └── main.jsx             # React DOM root mounting script
├── index.html               # Main HTML entry point
├── package.json             # NPM dependencies, scripts, and package details
├── postcss.config.js        # PostCSS configuration for Tailwind CSS
├── tailwind.config.js       # Tailwind CSS theme extension & design tokens
└── vite.config.js           # Vite bundler configuration
```

---

## 🌐 Deployment Instructions

### Option 1: Vercel Deployment (Recommended)

1. Push your project code to GitHub.
2. Sign in to [Vercel](https://vercel.com/) and click **"Add New Project"**.
3. Import your GitHub repository.
4. Vercel automatically detects **Vite**:
   - **Framework Preset**: Vite
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
5. Click **Deploy**.

---

### Option 2: Netlify Deployment

1. Sign in to [Netlify](https://www.netlify.com/) and select **"Add new site"** -> **"Import an existing project"**.
2. Connect your GitHub repository.
3. Configure build settings:
   - **Build Command**: `npm run build`
   - **Publish Directory**: `dist`
4. For client-side routing support, ensure a `public/_redirects` file exists with:
   ```text
   /*   /index.html   200
   ```
5. Click **Deploy Site**.

---

### Option 3: GitHub Pages Deployment

1. Update `vite.config.js` to set the `base` path:
   ```javascript
   export default defineConfig({
     base: '/food-picker-spinner/',
     plugins: [react()],
   })
   ```
2. Build static production bundle:
   ```bash
   npm run build
   ```
3. Deploy the contents of the `dist/` directory to your repository's `gh-pages` branch.

---

### Option 4: Docker & Nginx Deployment

You can containerize FoodSpin using Nginx to serve the built static bundle.

**`Dockerfile`**:
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

Build and run Docker container:
```bash
docker build -t food-picker-spinner .
docker run -p 8080:80 food-picker-spinner
```

---

## ⚖️ License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---

<p align="center">Made with ❤️ for food lovers and indecisive eaters everywhere.</p>
#   F o o d - P i c k e r - S p i n n e r  
 