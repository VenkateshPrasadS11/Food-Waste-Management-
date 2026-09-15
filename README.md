# 🌿 FoodLoop – Food Waste Management Platform

[![React](https://img.shields.io/badge/React-19-61dafb.svg?logo=react&logoColor=white)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-6-646cff.svg?logo=vite&logoColor=white)](https://vitejs.dev/)
[![Design](https://img.shields.io/badge/UI-Vanilla%20CSS%20Design%20System-16a34a.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

> **Reducing food waste. Feeding communities. Building a sustainable future.**  
> A full-featured web platform connecting surplus food donors (restaurants, caterers, hotels, households) with NGOs, shelters, and volunteer networks across Indian cities.

---

## 📌 Project Overview

Millions of tonnes of wholesome edible food are discarded daily from banquets, restaurants, hostels, and markets while millions face food insecurity. **FoodLoop** bridges this critical logistical gap by providing:

1. **Instant Surplus Food Reporting**: Quick donation logging with quantity, expiry timer, dietary tags, and pickup coordinates.
2. **Real-Time Surplus Marketplace**: Search, filter, and claim available hot meals, groceries, and bakery items before they expire.
3. **Hyperlocal Nearby Food Finder**: Interactive map visualization with city filters (Coimbatore, Chennai, Bangalore, Kochi, Madurai).
4. **Impact Dashboard & Analytics**: Data visualization powered by **Recharts** displaying meals rescued, carbon footprint prevented, and monthly redistribution trends.
5. **Food Safety & Quality Compliance**: Strict hygiene protocols aligned with FSSAI regulations to guarantee recipient health and dignity.
6. **Administrator Control Console**: Moderate listings, manage user roles, and monitor city-wide operations.

---

## 🚀 Key Features

### 🍲 1. Surplus Food Marketplace
- **Dynamic Search & Multi-Filters**: Filter by dietary category (Cooked Meals, Raw Groceries, Baked Goods, Packaged), City, and Meal Type (Breakfast, Lunch, Dinner).
- **Urgent Expiry Countdown**: Real-time relative timers calculating remaining safe consumption windows.
- **One-Click Claim System**: NGOs and shelters can reserve meals with instant contact exchange and verification modals.

### 📝 2. Seamless Donation Logging
- Step-by-step form capturing meal title, servings count, preparation timestamp, safe consumption window, dietary labels (Veg/Non-Veg), and pickup address.
- **Mandatory Hygiene Pledge**: Ensures donors certify proper storage and packaging before listing.

### 🗺️ 3. Interactive Location Map (OpenStreetMap & Leaflet)
- **Live Tile Map**: Powered by Leaflet and OpenStreetMap tiles (no paid API keys or external billing required).
- **Interactive Pins & Route Lines**: Displays food donations, recipient shelters, and real-time delivery vans with animated route polylines.
- **City Jump Controls**: Seamless fly-to navigation for **Coimbatore, Chennai, Bangalore, Kochi, and Madurai**.
- **Directions & Telemetry**: 1-click Google Maps navigation routing, food servings counts, and donor contacts.

### 🚚 4. Real-Time Food Deliveries Tracker (`/live-deliveries`)
- **Live Dispatch Radar**: Real-time ticker tracking total meals delivered today, active rescues in transit, and average door-to-door transit time.
- **Dynamic Delivery Simulation**: Live progress bars updating every 7 seconds across 4 stages: Assigned $\to$ Picked Up $\to$ In Transit $\to$ Delivered.
- **Volunteer Telemetry**: Driver names, contact dialers, vehicle numbers, cold-chain temperature logs (e.g. 68°C safe hold), and shelter delivery confirmation.
- **1-Click Rescue Spawner**: "Dispatch New Food Rescue" button to simulate and test on-demand food logistics.

### 📊 5. Donor & NGO Impact Dashboard
- **Recharts Integration**:
  - Weekly meals rescued bar chart.
  - Food category distribution pie chart.
  - CO₂ emission reduction trend line.
- Activity feed tracking claims, approvals, and volunteer handoffs.
- Export-ready summary metrics.

### 🛡️ 5. Food Safety Guidelines & Standards
- Dedicated 9-point hygiene rubric covering:
  - 2-Hour Room Temperature Rule
  - Sealed Food-Grade Packaging
  - Allergen & Dietary Labeling
  - Temperature Maintenance in Transit
  - Sensory Inspection Protocols

### 🔑 6. Multi-Role Demo Simulation
- Pre-seeded with realistic Indian mock data (Saravana Bhavan, Annapoorna Trust, Coimbatore Volunteer Network).
- Instant one-click test logins for:
  - **Food Donor** (Restaurateur / Event Caterer)
  - **NGO Representative** (Shelter Manager)
  - **System Administrator** (Moderator)

### 🌓 7. Premium UI/UX & Dark Mode
- Built with a bespoke **Vanilla CSS Design System** (1,800+ lines):
  - Emerald green & dark green forest theme (`#16a34a`, `#14532d`).
  - Google Fonts: **Inter** (body) & **Outfit** (headings).
  - Silky transitions, glassmorphism cards, skeleton loaders, and responsive layout for mobile, tablet, and desktop.
  - Dark mode toggle with persistent `localStorage` memory.

---

## 👥 Demo Login Credentials

For quick evaluation and demonstration, use the following pre-configured credentials:

| Role | Email | Password | Access / Capabilities |
| :--- | :--- | :--- | :--- |
| **Donor** | `arjun@demo.com` | `demo123` | Post surplus food, view donor dashboard, update profile |
| **NGO** | `hope@demo.com` | `demo123` | Claim surplus listings, view distribution records |
| **Volunteer**| `priya@demo.com` | `demo123` | View nearby pickup points, logistics coordination |
| **Admin** | `admin@foodloop.demo` | `admin123` | Full console: moderate listings, toggle users, reset database |

> *Tip: You can also use the **"⚡ Instant Demo Profiles"** buttons on the Login page to sign in with a single click.*

---

## 👨‍💻 Founder & Contact

- **Founder**: Venkatesh Prasad
- **Gmail**: [venkateshprasad1108@gmail.com](mailto:venkateshprasad1108@gmail.com)
- **Contact / WhatsApp**: `+91 9342178826` / `9342178826`
- **Top Right Navigation Button**: Click **"Contact founder:"** in the top-right navbar anywhere in the app to view direct contact details, copy email/phone, or send a direct message.
- **Automated Login Alert**: Every time a user logs into FoodLoop, an automated security notification is routed to `venkateshprasad1108@gmail.com` with user session details.

---

## 🛠️ Technology Stack

- **Frontend Framework**: [React 19](https://react.dev/) + [Vite](https://vitejs.dev/)
- **Styling**: Modern Vanilla CSS with CSS custom properties (variables), Flexbox/Grid, and Dark Mode
- **Icons**: [Lucide React](https://lucide.dev/) + Optimized inline SVGs
- **Data Visualization**: [Recharts](https://recharts.org/)
- **Routing**: [React Router DOM v6](https://reactrouter.com/)
- **Data Persistence**: Browser `localStorage` (No external backend or paid API keys required)

---

## 📦 Getting Started Locally

### Prerequisites
- Node.js (v18 or higher recommended)
- npm or yarn

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/foodloop.git
   cd foodloop
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the local development server**:
   ```bash
   npm run dev
   ```

4. **Open in browser**:
   Navigate to `http://localhost:5173/` (or the URL shown in your terminal).

### Build for Production
```bash
npm run build
```
The compiled, production-ready assets will be located in the `dist/` directory.

---

## 📁 Project Architecture

```
moonlight 2/
├── index.html               # Main HTML entry with Google Fonts
├── package.json             # Project dependencies & scripts
├── vite.config.js           # Vite build configuration
├── src/
│   ├── main.jsx             # React entry point
│   ├── App.jsx              # React Router setup & global layout
│   ├── index.css            # Complete CSS design system & tokens
│   │
│   ├── context/
│   │   └── AppContext.jsx   # Theme, user auth state, and toast notifications
│   │
│   ├── data/
│   │   └── sampleData.js    # Pre-seeded Indian dishes, donors, NGOs, and metrics
│   │
│   ├── utils/
│   │   └── localStorage.js  # CRUD helpers for donations, users, claims, and theme
│   │
│   ├── components/
│   │   ├── Navbar.jsx       # Responsive sticky navbar + dark mode toggle
│   │   ├── Footer.jsx       # Footer with links, emergency helpline, socials
│   │   ├── FoodCard.jsx     # Reusable food card with countdown & claim modal
│   │   ├── StatsCard.jsx    # Animated metric counters
│   │   ├── Modal.jsx        # Reusable modal with backdrop & accessibility
│   │   ├── Toast.jsx        # Floating notifications container
│   │   └── SkeletonLoader.jsx # Polished loading skeletons
│   │
│   └── pages/
│       ├── Home.jsx         # Landing page with hero, live counters, and CTA
│       ├── About.jsx        # Mission, timeline, team, and 9-point safety rubric
│       ├── HowItWorks.jsx   # 4-step workflow for donors, NGOs, and volunteers
│       ├── SurplusFood.jsx  # Marketplace with search, 4 filters, and sort
│       ├── Donate.jsx       # Donation logging form with validation
│       ├── FindFood.jsx     # Hyperlocal map placeholder and pin directory
│       ├── Dashboard.jsx    # Analytics with Recharts, my donations, and claims
│       ├── Profile.jsx      # User profile, emoji avatar picker, security
│       ├── Contact.jsx      # Inquiries, emergency hotline, and FAQ accordion
│       ├── Login.jsx        # Sign-in with one-click demo credentials
│       ├── Register.jsx     # Multi-role registration with pledge agreement
│       └── Admin.jsx        # Admin moderation, user toggles, and data reset
└── README.md
```

---

## 📜 Food Safety Compliance

Food safety is at the core of FoodLoop. Donors and volunteers are guided by clear protocols:
- **Time-Temperature Control**: Cooked foods must be transferred within 2 to 4 hours of preparation.
- **Hygiene Verification**: Food items must be sealed in non-toxic, food-grade containers.
- **Transparency**: Every listing must state preparation date, exact time, and any allergens (dairy, nuts, gluten).

---

## 🎓 Academic Portfolio Note

This web application was engineered as a comprehensive mini-project for a computer science / software engineering portfolio. It demonstrates:
- Component-driven UI development and state management in React.
- Advanced client-side data persistence with browser storage.
- Interactive charting and data visualization.
- Complete responsive design without reliance on heavy UI frameworks like Tailwind or Bootstrap.
- Practical software engineering solving real-world Sustainable Development Goals (SDG 2: Zero Hunger & SDG 12: Responsible Consumption).

---

## 📄 License

This project is licensed under the MIT License — feel free to use and adapt it for educational and community purposes.
