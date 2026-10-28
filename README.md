# e-plantShopping: Paradise Nursery Shopping Application

**Project Name:** e-plantShopping  
**Application Title:** Paradise Nursery Shopping Application  

---

## Project Overview

**e-plantShopping** is a modern, responsive e-commerce web application developed for **Paradise Nursery**, an online plant nursery where green meets serenity. Built using **React**, **Redux Toolkit**, and **Vite**, the **e-plantShopping** application provides a comprehensive shopping experience allowing users to browse diverse plant collections, view product details, manage their shopping carts dynamically, and compute prices in real-time.

The **e-plantShopping** project emphasizes interactive frontend features including:
- An engaging landing page with company branding and background imagery.
- An About Us section detailing Paradise Nursery's mission and team of experts.
- A categorized plant catalog containing 5 distinct categories with 6 unique plants per category.
- Dynamic cart state management with real-time addition, removal, and quantity adjustment.
- A consistent navigation bar with navigation links to Home, Plants, and Cart with live count display.

---

## Key Features

- **Project Name Details**: Titled **e-plantShopping** (Paradise Nursery Shopping Application).
- **Company Introduction (`AboutUs.jsx`)**: Comprehensive overview of Paradise Nursery's passion for quality plants and commitment to a greener lifestyle.
- **Hero Landing Page (`App.jsx` & `App.css`)**: Beautiful greenhouse background styling with translucent overlay, company name branding, and a "Get Started" call-to-action button that transitions smoothly into the store.
- **Global State Management (`CartSlice.jsx`)**: Redux Toolkit slice managing cart state with three core reducer functions:
  - `addItem`: Adds selected houseplants to the cart or increments their quantity if already present.
  - `removeItem`: Removes a plant item from the shopping cart.
  - `updateQuantity`: Adjusts the quantity of items directly when incremented or decremented.
- **Houseplant Catalog (`ProductList.jsx`)**:
  - Displays at least 6 unique houseplants per category across 5 distinct categories (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, Low Maintenance).
  - "Add to Cart" button that dispatches items to the Redux store, disables once added, and displays "Added to Cart".
  - Persistent navbar on both Product Listing and Cart pages with navigation links for Home (`handleParadiseNurseyClick`), Plants, and Cart.
  - Dynamic cart counter showing total number of items, updating automatically when items are added or removed.
- **Shopping Cart Page (`CartItem.jsx`)**:
  - Displays plant thumbnail, name, unit price, quantity controls (`+` and `-`), and total cost per plant.
  - Calculates and displays the total cart amount for all plants.
  - Quick-remove "Delete" button per item.
  - "Continue Shopping" button to return to the plant listing.
  - "Checkout" button that alerts a "Coming Soon" notification message.

---

## Project Structure

```text
e-plantShopping/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   ├── AboutUs.css          # Styling for the About Us section
│   ├── AboutUs.jsx          # Company mission and details component
│   ├── App.css              # Landing page styling and background image
│   ├── App.jsx              # Landing page with company name & Get Started button
│   ├── CartItem.css         # Styling for shopping cart interface
│   ├── CartItem.jsx         # Shopping cart page component with totals & actions
│   ├── CartSlice.jsx        # Redux Toolkit slice (addItem, removeItem, updateQuantity)
│   ├── index.css            # Global resets and fonts
│   ├── main.jsx             # React entry point with Redux Provider
│   ├── ProductList.css      # Styling for navbar, product grid, and cards
│   ├── ProductList.jsx      # Plant listing page, categories, and persistent navbar
│   └── store.js             # Redux store configuration
├── index.html
├── package.json
├── README.md                # Project documentation and details (e-plantShopping)
└── vite.config.js
```

---

## Technologies Used

- **React 18**: Component-driven user interface.
- **Redux Toolkit & React-Redux**: Global state management for cart operations.
- **Vite**: Rapid frontend build tooling and development environment.
- **CSS3**: Modern responsive layouts with flexbox, grid, and CSS media queries.

---

## Getting Started

### Prerequisites
- Node.js (v16.0 or higher recommended)
- npm or yarn

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/syedraihanm/e-plantShopping.git
   cd e-plantShopping
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the development server:
   ```bash
   npm run dev
   ```
4. Build for production:
   ```bash
   npm run build
   ```

---

## License
This project is open-source and available under the MIT License.
