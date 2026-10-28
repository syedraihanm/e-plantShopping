# Paradise Nursery Shopping Application

A modern, responsive e-commerce web application for **Paradise Nursery**, an online plant store where green meets serenity. Built using **React**, **Redux Toolkit**, and **Vite**, this application offers an engaging shopping experience enabling users to explore diverse plant collections, manage their shopping carts, and calculate costs seamlessly in real-time.

---

## Project Overview

**Paradise Nursery** is dedicated to bringing nature closer to homes and workplaces. The application consists of:
1. **Landing Page**: An inviting entrance featuring high-resolution greenhouse imagery, company branding, a mission statement via the About Us section, and a "Get Started" call-to-action button.
2. **Product Listing Page**: An organized showcase featuring houseplants categorized into multiple sections (Air Purifying, Aromatic Fragrant, Insect Repellent, Medicinal, and Low Maintenance). Each plant displays its thumbnail image, name, description, and price with an interactive "Add to Cart" button.
3. **Responsive Navigation Bar**: Persistent navigation across both the product catalog and shopping cart views, displaying quick links to Home, Plants, and a dynamic Cart icon displaying the live total count of items.
4. **Shopping Cart Page**: A full-featured shopping cart view displaying added plants with thumbnails, unit prices, subtotal cost per plant, and overall cart total. Users can increment, decrement, or remove items, proceed to checkout, or continue browsing plants.

---

## Key Features

- **Company Introduction (`AboutUs.jsx`)**: Comprehensive overview of Paradise Nursery's passion for quality plants and customer service.
- **Hero Landing (`App.jsx` & `App.css`)**: Beautiful background styling with translucent overlay, branding, and intuitive smooth transition into the plant shop.
- **Global State Management (`CartSlice.jsx`)**: Built with Redux Toolkit to cleanly manage cart operations:
  - `addItem`: Adds selected houseplants to the cart or increments existing quantity.
  - `removeItem`: Deletes an item from the cart.
  - `updateQuantity`: Updates the quantity when users increment or decrement items.
- **Houseplant Catalog (`ProductList.jsx`)**:
  - Displays at least 6 unique houseplants per category across 5 distinct categories.
  - Dynamic "Add to Cart" button that disables and displays "Added to Cart" once an item is in the cart.
  - Real-time cart badge counter that automatically reflects the total item count.
  - Integrated navigation bar with links to Home, Plants, and Cart.
- **Cart Management (`CartItem.jsx`)**:
  - Displays unit price, item thumbnail, quantity controls, and total cost per plant.
  - Dynamically calculates grand total cost for all items in the cart.
  - Quantity controls (`+` and `-`) with auto-removal if quantity reaches zero.
  - Quick-remove "Delete" button per item.
  - "Continue Shopping" button to return to the catalog and a "Checkout" button informing users that order placement is coming soon.

---

## Project Structure

```text
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   ├── AboutUs.css          # Styling for the About Us section
│   ├── AboutUs.jsx          # Company mission and background component
│   ├── App.css              # Landing page layout and background styling
│   ├── App.jsx              # Main application root and view controller
│   ├── CartItem.css         # Styling for shopping cart interface
│   ├── CartItem.jsx         # Cart display, item totals, and quantity controls
│   ├── CartSlice.jsx        # Redux Toolkit slice with addItem, removeItem, and updateQuantity
│   ├── index.css            # Global resets and fonts
│   ├── main.jsx             # React entry point with Redux Provider
│   ├── ProductList.css      # Styling for navbar, product grid, and cards
│   ├── ProductList.jsx      # Plant catalog and persistent navigation bar
│   └── store.js             # Redux store configuration
├── index.html
├── package.json
├── README.md                # Project documentation and details
└── vite.config.js
```

---

## Technologies Used

- **React 18**: Component-based UI architecture.
- **Redux Toolkit & React-Redux**: Centralized global application state.
- **Vite**: Ultra-fast build and development tool.
- **CSS3**: Responsive flexbox and grid styling with responsive media queries.

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
