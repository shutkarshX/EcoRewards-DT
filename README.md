# EcoRewards — Campus Sustainability & Waste Segregation Platform

[![React](https://img.shields.io/badge/React-18-61DAFB.svg)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF.svg)](https://vitejs.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2022-F7DF1E.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![SDG 12](https://img.shields.io/badge/SDG%2012-Responsible%20Consumption-BF8B2E.svg)](https://sdgs.un.org/goals/goal12)
[![Design Thinking](https://img.shields.io/badge/Methodology-Design%20Thinking%20PBL-brightgreen.svg)]()

A gamified web platform prototype developed for the **Design Thinking (DT)** Project-Based Learning (PBL) curriculum. It addresses campus waste mismanagement by transforming waste segregation into a rewarding, habit-forming experience through eco-points, canteen vouchers, and interactive awareness quizzes.

---

## 💡 The Design Thinking Journey

```mermaid
flowchart LR
    E["1. Empathize<br/>Observed unsegregated campus dustbins & lack of student incentive."] --> D["2. Define<br/>'How might we make waste segregation tangible, visible, and rewarding?'"]
    D --> I["3. Ideate<br/>Gamified eco-points, canteen redemptions, and micro-quizzes."]
    I --> P["4. Prototype<br/>Reactive web app with waste logging, rewards store & leaderboard."]
    P --> T["5. Test<br/>Interactive prototype evaluated for usability & engagement."]
```

---

## 🏛️ Application Architecture & User Flow

```mermaid
graph TD
    User([Campus Student])

    subgraph Platform["EcoRewards Web Application"]
        Logger["Waste Disposal Logger<br/>(Dry / Wet / Plastic + Weight)"]
        Calculator["Eco-Point Calculator<br/>(10 Points / Kg)"]
        Store["Rewards Redemption Store<br/>(Canteen & Stationery Vouchers)"]
        Quiz["Segregation Literacy Quiz<br/>(Interactive Waste Sorting)"]
        Leaderboard["Campus Leaderboard<br/>(Rankings & Peer Motivation)"]
    end

    User -->|"1. Segregates & Logs Waste"| Logger
    Logger --> Calculator
    Calculator -->|"Credits Points"| Store
    User -->|"2. Tests Knowledge"| Quiz
    Quiz -->|"Earns Bonus Points"| Calculator
    Calculator -->|"Updates Score"| Leaderboard
    Store -->|"Redeems Perks"| User
```

---

## ✨ Core Features

1. **Smart Waste Logging**:
   * Three distinct disposal categories: **Dry** (paper/cardboard/metal), **Wet** (organic/food), and **Plastic** (bottles/packaging).
   * Weight-based calculation converting grams directly to earned eco-points.
   * Daily submission limits preventing fraudulent submissions.

2. **Gamified Rewards Store**:
   * Redeemable perks including campus canteen vouchers, free snacks/coffee, stationery packs, and bookstore credits.
   * Real-time stock tracking for available rewards.

3. **Waste Literacy Quiz**:
   * Interactive micro-quizzes testing knowledge on correct bin placement (e.g., electronic items, compostable packaging).
   * Instant feedback and educational explanations.

4. **Campus Leaderboard**:
   * Student rank tracking showcasing top eco-contributors across departments.
   * Fosters constructive social motivation and environmental accountability.

---

## 🚀 Running Locally

### Prerequisites
* **Node.js**: 18+ and `npm`

### Setup Steps

```bash
# Clone the repository
git clone https://github.com/shutkarshX/EcoRewards.git
cd EcoRewards

# Install project dependencies
npm install

# Start the Vite development server
npm run dev
```

*Open `http://localhost:5173` in your browser to interact with the application.*

### Production Build

```bash
# Compile optimized production bundle
npm run build

# Preview production build locally
npm run preview
```

---

## 📂 Repository Structure

```text
EcoRewards/
├── src/
│   ├── App.jsx                # Main gamified application (UI, Quiz, Store, Leaderboard)
│   ├── main.jsx               # React DOM root mounting
│   └── index.css              # Global styles & layout variables
├── index.html                 # HTML shell
├── vite.config.js             # Vite build configuration
├── package.json               # NPM scripts and dependencies
├── .gitignore
└── README.md
```

---

## 📜 Academic Curriculum Mapping
* **Subject:** Design Thinking (DT).
* **Focus Area:** Environmental Sustainability, Campus Waste Management, Behavior Design & Gamification, User-Centric Prototyping.
