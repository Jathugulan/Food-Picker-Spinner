# 🍕 Food Picker Spinner — FoodSpin

<p align="center">
  <img src="https://img.shields.io/badge/FoodSpin-Food%20Picker%20Spinner-orange?style=for-the-badge" alt="FoodSpin">
  <img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React 19">
  <img src="https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite">
  <img src="https://img.shields.io/badge/Tailwind%20CSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Framer%20Motion-11-EF008C?style=for-the-badge" alt="Framer Motion">
  <img src="https://img.shields.io/badge/Recharts-2-22C55E?style=for-the-badge" alt="Recharts">
  <img src="https://img.shields.io/badge/Netlify-Deployed-00C7B7?style=for-the-badge&logo=netlify&logoColor=white" alt="Netlify">
</p>

<p align="center">
  <strong>🎯 Spin. Decide. Enjoy.</strong>
</p>

<p align="center">
  A modern, interactive and responsive food decision-making web application that helps users quickly decide what to eat using a fun spinning wheel experience.
</p>

<p align="center">
  🌐 <strong>Live Demo:</strong>
  <a href="https://food-picker-spinner.netlify.app">
    https://food-picker-spinner.netlify.app
  </a>
</p>

---

## 📖 About FoodSpin

**Food Picker Spinner (FoodSpin)** is a modern Single Page Application designed to solve the everyday problem of:

> **"What should I eat today?" 🍕🍔🍜**

Instead of endlessly thinking about food choices, users can manage their food collection, organize foods into categories, spin an interactive wheel, view previous results, and analyze their food-selection statistics.

FoodSpin uses a client-side architecture with browser-based data persistence through `localStorage`, so users can maintain their food data and history without requiring a traditional backend server.

---

# ✨ Key Features

## 🎯 1. Interactive Food Spinner

The main feature of FoodSpin is the interactive food-selection wheel.

### Features

* 🎡 Animated spinning wheel
* 🍕 Food items displayed as wheel segments
* 🎲 Random food selection
* ⚡ Smooth spin animation
* 🎯 Accurate winner positioning
* 🔄 Multiple full rotations
* 🌀 Realistic acceleration and deceleration
* ✨ Animated visual feedback
* 🏆 Winner/result display
* 📱 Fully responsive spinner
* 👆 Touch-friendly controls

The spinner uses segment-based angular calculations to distribute food items across a 360° wheel.

For `N` food items:

```text
Segment Angle = 360° / N
```

---

# 🍔 2. Food Management

Users can manage their personal food collection.

### Food Management Features

* ➕ Add new food
* ✏️ Edit food
* 🗑️ Delete food
* ❤️ Mark food as favorite
* ⭐ Add food rating
* 🏷️ Add food tags
* 📝 Add food descriptions
* 📂 Assign categories
* 🔍 Manage available food choices
* 🎯 Use foods in the spinner

Example food information:

```text
Name
Category
Emoji
Description
Favorite
Rating
Tag
```

---

# 📂 3. Category Management

Organize food items into meaningful categories.

### Features

* ➕ Create categories
* ✏️ Edit categories
* 🗑️ Delete categories
* 🍔 Food grouping
* 🎯 Category-based food selection
* 📊 Category statistics
* 🧩 Easy food organization

Example categories:

```text
🍕 Pizza
🍔 Burgers
🍜 Asian
🍛 Rice
🥗 Healthy
🍰 Desserts
🥤 Drinks
```

---

# 🕘 4. Spin History

FoodSpin records previous spinner results using browser storage.

### Features

* 🕘 View previous results
* 🍕 Display selected food
* 📅 Track selection history
* 🔍 Review previous decisions
* 🗑️ Clear history
* 📊 Use history for statistics

History remains available after refreshing the browser because the application uses `localStorage`.

---

# 📊 5. Statistics Dashboard

The statistics page provides visual insights into food selections.

### Features

* 📈 Selection statistics
* 📊 Food selection frequency
* 🏆 Most selected foods
* 📂 Category statistics
* 📉 Historical data visualization
* 📊 Interactive charts
* 🔢 Total spin statistics
* 🎯 Food preference insights

Charts are implemented using **Recharts**.

---

# 🏠 6. Modern Home Dashboard

The home page provides a quick overview of the application.

### Includes

* 🎯 Quick Spin action
* 🍕 Food overview
* 📂 Category overview
* 🕘 Recent history
* 📊 Statistics overview
* ❤️ Favorite foods
* ⚡ Quick navigation
* ✨ Modern animations

---

# 🌙 7. Theme Support

FoodSpin provides a modern visual experience with theme support.

### Supported Modes

* ☀️ Light Mode
* 🌙 Dark Mode
* 🖥️ System/Auto Mode

The interface uses custom Tailwind theme tokens for backgrounds, cards, gradients and interactive components.

---

# 📱 8. Fully Responsive Design

FoodSpin is designed to work across different screen sizes.

### Supported Devices

| Device            | Support |
| ----------------- | ------- |
| 📱 Mobile         | ✅       |
| 📱 Large Mobile   | ✅       |
| 📲 Tablet         | ✅       |
| 💻 Laptop         | ✅       |
| 🖥️ Desktop       | ✅       |
| 🖥️ Large Desktop | ✅       |

### Responsive Features

* 📱 Mobile-first layouts
* 🍔 Responsive navigation
* 🎡 Responsive spinner
* 🃏 Responsive cards
* 📊 Responsive charts
* 👆 Touch-friendly controls
* 📐 Flexible grids
* 🔄 Adaptive spacing
* 🖼️ Responsive content
* 🚫 No unnecessary horizontal scrolling

---

# 💾 9. Local Storage Persistence

FoodSpin does not require a backend database for its core functionality.

Data is stored locally in the browser using:

```javascript
localStorage
```

### Stored Data

```text
foodspin_foods
foodspin_categories
foodspin_history
```

This allows users to:

* Save food items
* Save categories
* Save spinner history
* Maintain preferences
* Keep data after page refresh

---

# ⚡ 10. Performance Optimization

FoodSpin is designed as a lightweight client-side application.

### Performance Features

* ⚡ Vite production builds
* 📦 Optimized static assets
* 🚀 Fast page loading
* 🧩 Component-based architecture
* 💾 Client-side persistence
* 🎨 Efficient Tailwind styling
* 🌀 Optimized animations
* 📱 Responsive rendering
* 🔄 SPA navigation

---

# 🎨 11. Premium UI/UX

FoodSpin follows a modern application design system.

### UI Features

* ✨ Modern cards
* 🌈 Gradient accents
* 🪟 Glass-style surfaces
* 🌙 Dark mode
* 🎯 Clear visual hierarchy
* 🧩 Consistent components
* 🔄 Smooth transitions
* 💫 Micro-interactions
* 📱 Mobile-friendly controls
* 🎨 Modern typography
* 🧭 Intuitive navigation

---

# 🧭 Application Pages

FoodSpin contains the following major pages:

| Page          | Description              |
| ------------- | ------------------------ |
| 🏠 Home       | Application dashboard    |
| 🎡 Spinner    | Interactive food picker  |
| 🍔 Foods      | Manage food items        |
| 📂 Categories | Manage food categories   |
| 📊 Statistics | Food selection analytics |
| 🕘 History    | Previous spin results    |
| ⚙️ Settings   | Application preferences  |

---

# 🖼️ Screenshots

## 🏠 Home

![FoodSpin Home](screenshots/home.jpg)

---

## 🎡 Food Spinner

![FoodSpin Spinner](screenshots/spinner.jpg)

---

## 🍔 Foods

![FoodSpin Foods](screenshots/foods.jpg)

---

## 📂 Categories

![FoodSpin Categories](screenshots/categories.jpg)

---

## 📊 Statistics

![FoodSpin Statistics](screenshots/statistics.jpg)

---

## 🕘 History

![FoodSpin History](screenshots/history.jpg)

---

# 🏗️ System Architecture

FoodSpin follows a client-side React architecture.

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
              ┌───────────────┐
              │ Custom Hooks  │
              │ useLocalStorage│
              └───────┬───────┘
                      │
                      ▼
              ┌───────────────┐
              │  localStorage │
              └───────────────┘
```

---

# 📁 Project Structure

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
│   │
│   ├── components/
│   │   └── SpinnerWheel.jsx
│   │
│   ├── hooks/
│   │   └── useLocalStorage.js
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
│   │   └── spinnerUtils.js
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

# 🧮 Spinner Algorithm

FoodSpin dynamically divides the wheel into equal segments.

For `N` active food items:

```text
θ = 360° / N
```

Each food receives one segment.

The application calculates:

```text
Start Angle
End Angle
Center Angle
Target Rotation
```

The selected food is then aligned with the pointer after the animation.

---

# 🌀 Spinner Animation

The spinner uses **Framer Motion** for smooth animation.

The animation includes:

* Multiple full rotations
* Fast initial movement
* Progressive deceleration
* Final pointer alignment
* Randomized landing position
* Smooth transition
* Visual winner feedback

This creates a more natural spinning-wheel experience instead of simply changing the selected food instantly.

---

# 🧰 Technology Stack

## Frontend

* ⚛️ React 19
* ⚡ Vite 5
* 🎨 Tailwind CSS 3
* 🌀 Framer Motion 11
* 📊 Recharts 2
* 🧭 React Router
* 🟨 JavaScript ES6+

## Browser APIs

* `localStorage`
* SVG
* Web Storage API

## Deployment

* 🐙 GitHub
* 🌐 Netlify

---

# 📦 Installation

## 1. Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

## 2. Enter Project

```bash
cd FoodSpin
```

## 3. Install Dependencies

```bash
npm install
```

## 4. Start Development Server

```bash
npm run dev
```

Open the local development URL shown by Vite.

---

# 🏭 Production Build

Create an optimized production build:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

---

# 🚀 Netlify Deployment

FoodSpin is deployed using Netlify.

### Build Configuration

```text
Branch:
main

Build command:
npm run build

Publish directory:
dist

Base directory:
empty

Functions directory:
empty
```

### 🌐 Live Website

**FoodSpin Live Demo:**

https://food-picker-spinner.netlify.app

---

# 🔄 Deployment Workflow

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
Push to main
    │
    ▼
Netlify Build
    │
    ▼
npm run build
    │
    ▼
dist/
    │
    ▼
Netlify CDN
    │
    ▼
🌐 Live FoodSpin Website
```

---

# 🔐 Privacy

FoodSpin is designed as a client-side application.

Core food data and spinner history are stored locally in the user's browser.

No backend server is required for the application's core food-selection functionality.

---

# 🧪 Testing & Validation

The application should be validated across:

### Desktop

```text
1280 × 850
```

### Tablet

```text
768 × 1024
```

### Mobile

```text
375 × 812
```

### Validation Areas

* ✅ Production build
* ✅ Page navigation
* ✅ Spinner functionality
* ✅ Food CRUD operations
* ✅ Category management
* ✅ History persistence
* ✅ Statistics
* ✅ Theme switching
* ✅ Responsive layouts
* ✅ Mobile navigation
* ✅ Browser refresh behavior

---

# 📈 Performance

The project technical analysis reports a production build consisting of optimized Vite assets.

Reported build package:

```text
Total Build Package: 494.96 kB
Gzip Size:            139.80 kB
```

The report also records:

```text
Performance Score: 98/100
FCP:               0.4s
LCP:               0.8s
CLS:               0.00
TBT:               0ms
```

> Performance results can vary depending on browser, device, network conditions and deployment environment.

---

# 🎯 Project Goals

FoodSpin was created to:

* Reduce food decision fatigue
* Make food selection entertaining
* Provide a simple food-management system
* Help users organize food choices
* Provide useful selection statistics
* Maintain spin history
* Deliver a responsive modern UI
* Provide a fast client-side experience

---

# 💡 Future Enhancements

Potential future improvements include:

* 🤖 AI food recommendations
* 🌦️ Weather-based food suggestions
* 📍 Location-based restaurant recommendations
* 🥗 Nutrition information
* ❤️ Advanced favorites
* 🔐 User authentication
* ☁️ Cloud synchronization
* 📱 PWA support
* 🔔 Notifications
* 🎵 Spinner sound effects
* 🌎 Multi-language support
* 📤 Data export/import
* 📊 Advanced analytics
* 👥 Shared food lists
* 🎨 Custom spinner themes

---

# 🏆 Project Highlights

```text
✨ Modern Premium UI
🎡 Interactive Food Spinner
🍔 Complete Food Management
📂 Category Management
🕘 Spin History
📊 Statistics Dashboard
🌙 Theme Support
📱 Fully Responsive
💾 LocalStorage Persistence
⚡ Vite Performance
🌀 Framer Motion Animations
📈 Recharts Analytics
🚀 Netlify Deployment
🔒 Client-Side Privacy
```

---

# 🤝 Contributing

Contributions are welcome.

```bash
# Fork the repository

# Create a feature branch
git checkout -b feature/new-feature

# Commit changes
git add .
git commit -m "feat: add new feature"

# Push branch
git push origin feature/new-feature
```

Then open a Pull Request.

---

# 🐛 Issues & Feedback

If you find a bug or have a feature suggestion:

1. Open an issue on GitHub
2. Describe the problem clearly
3. Include reproduction steps
4. Add screenshots when useful
5. Suggest an improvement if possible

---

# 📄 License

This project is intended for educational and portfolio purposes.

---

# 👨‍💻 Author

## Raveendran Jathugulan

**Full-Stack Developer | MERN Stack Developer | BICT Undergraduate**

Passionate about building modern, responsive and user-friendly web applications.

---

# 🌐 Connect

* 🐙 GitHub: [Jathugulan](https://github.com/Jathugulan)
* 💼 LinkedIn: [Raveendran Jathugulan](https://www.linkedin.com/in/raveendran-jathugulan/)
* 🌐 Live Project: [FoodSpin](https://food-picker-spinner.netlify.app)

---

# ⭐ Support

If you like **FoodSpin**, please consider giving the repository a ⭐ on GitHub.

<p align="center">
  <strong>🍕 Spin Your Way to Your Next Meal! 🎡</strong>
</p>

<p align="center">
  Made with ❤️ using React, Vite & Tailwind CSS
</p>
