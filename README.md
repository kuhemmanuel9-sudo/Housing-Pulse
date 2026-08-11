# 🏠 Housing Pulse — U.S. Housing Market Dashboard

Housing Pulse is an interactive front-end dashboard that explores **simulated residential property data across all 50 U.S. states**. I built it as a portfolio project to practice data modeling, responsive UI design, filtering, client-side state management, visualization, and export functionality.

> **Important:** The properties and prices in this project are synthetic. They are generated for learning and demonstration and are **not live MLS, Zillow, Redfin, assessor, or lender data**.

## 🌎 Coverage

The app includes a structured property dataset covering **all 50 states**. Each state has multiple simulated records, with different cities, property types, prices, bedroom counts, square footage, and years built.

The current demo generates **200 simulated properties (4 per state)** so the interface can demonstrate real filtering and comparison behavior without pretending to provide an incomplete or fake “live listings” feed.

## ✨ Features

- All **50 states** represented in the dataset
- 200 simulated property records
- Search by address, city, state, ZIP, or state name
- Filter by state, property type, and price range
- Quick filters for favorites, newer homes, affordable homes, and luxury homes
- Sort by price, city, state, and bedrooms
- Responsive cards for desktop, tablet, and mobile
- Light / dark theme with local persistence
- Favorites stored in `localStorage`
- Compare up to four properties
- Property detail modal with simulated price history visualization
- CSV export for the full synthetic dataset
- Lazy-loaded property images
- Accessible labels and descriptive status text
- Clear synthetic-data disclaimer throughout the app

## 🧰 Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript
- CSS Grid / Flexbox
- SVG-free CSS bar charts
- `localStorage` for saved preferences
- GitHub Pages compatible

## 🚀 Run Locally

No build system or package installation is required.

```bash
git clone https://github.com/kuhemmanuel9-sudo/Travel-price-dashboard.git
cd Travel-price-dashboard
```

Open `index.html` in a modern browser, or serve the folder with any static HTTP server.

## 📁 Project Structure

```text
Housing-Pulse/
├── index.html
└── README.md
```

The current version intentionally keeps the app dependency-free so it is easy to inspect and deploy.

## 📊 How the Data Works

The property records are generated from a state-level configuration containing:

- State abbreviation and full name
- Representative city
- Base property price
- Property type
- Bedrooms and bathrooms
- Square footage
- Year built
- Sample image

A deterministic daily variation is applied to the base price so the dashboard can demonstrate changing market values without presenting the result as real-world data.

## 🔒 Data Transparency

This project does **not** claim to provide real estate listings or live market data.

The buttons and interface are intentionally designed as a realistic dashboard prototype. A production version could replace the synthetic data layer with licensed APIs, MLS feeds, public assessor data, or another authorized source.

## 🔮 Possible Next Steps

- Connect to a licensed real-estate API
- Add an interactive U.S. map
- Add county / metro-level analysis
- Add mortgage and affordability calculators
- Add rental market mode
- Add historical market series from authorized sources
- Add authentication and saved dashboards
- Add backend caching and API rate-limit handling
- Add automated tests and CI/CD

## 👤 About

Built by **Emmanuel Kuh** as a portfolio project focused on analytics, interactive dashboards, data visualization, and practical web development.

- GitHub: https://github.com/kuhemmanuel9-sudo
- LinkedIn: add your profile link here

## 📄 License

MIT License — use, modify, and share the project with attribution.

---

**Note:** “All 50 states” means the demo contains coverage for every U.S. state. It does **not** mean every individual property in the United States, which would require a live property-data source and a substantially different data architecture.
