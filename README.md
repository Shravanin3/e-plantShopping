# Paradise Nursery Shopping Application

Paradise Nursery is an interactive, modern e-commerce web application for plant enthusiasts, designed to bring nature closer to homes and offices. Built with **React** and **Redux Toolkit**, this application allows users to browse a diverse collection of houseplants, explore plant details and categories, add plants to a shopping cart, dynamically manage quantities, and calculate total costs in real-time.

---

## Project Overview

- **Project Name:** Paradise Nursery Shopping Application (e-plantShopping)
- **Course:** Developing Front-End Apps with React (IBM / Coursera)
- **Author:** Shravanin3

---

## Features

### 1. Landing Page
- Striking greenhouse nursery background image and aesthetic glassmorphism styling.
- Clear branding featuring company name (**Paradise Nursery**) and tagline (*"Where Green Meets Serenity"*).
- **About Us** section introducing the nursery's mission, expert plant care standards, and commitment to environmental well-being.
- **Get Started** button providing a seamless transition to the plant catalog.

### 2. Product Catalog (`ProductList.jsx`)
- Over 30 unique houseplants categorized into 5 distinct collections:
  - **Air Purifying Plants** (Snake Plant, Spider Plant, Peace Lily, Boston Fern, Rubber Plant, Aloe Vera)
  - **Aromatic Fragrant Plants** (Lavender, Jasmine, Rosemary, Mint, Lemon Balm, Hyacinth)
  - **Insect Repellent Plants** (Oregano, Marigold, Geraniums, Basil, Lavender, Catnip)
  - **Medicinal Plants** (Aloe Vera, Echinacea, Peppermint, Lemon Balm, Chamomile, Calendula)
  - **Low Maintenance Plants** (ZZ Plant, Pothos, Snake Plant, Cast Iron Plant, Succulents, Aglaonema)
- Each plant card displays a high-resolution thumbnail image, plant name, description, and unit price.
- **Add to Cart** functionality:
  - Adds the selected plant to the Redux shopping cart state.
  - Dynamically disables the button and updates the button label to **"Added to Cart"**.
  - Dynamically increments the cart icon badge count in the navigation bar.

### 3. Responsive Navigation Bar
- Consistent navigation header accessible on both the Product Listing and Shopping Cart views.
- **Brand Link / Home:** Seamlessly returns the user to the landing page.
- **Plants Link:** Allows quick return to the product catalog from the cart.
- **Cart Icon & Badge:** Features a shopping cart icon with a live badge showing the total count of items in the cart.

### 4. Shopping Cart (`CartItem.jsx` & `CartSlice.jsx`)
- Detailed cart table/cards showing thumbnail image, plant name, and unit price for every added item.
- Quantity adjustment buttons (**`+`** and **`-`**) to increment or decrement individual item quantities.
  - Decreasing quantity to 0 automatically removes the plant from the cart.
- Subtotal cost calculation for each line item (`Unit Price × Quantity`).
- Total cart amount dynamically calculated and updated across all items.
- **Delete Button:** Allows complete removal of a plant item from the cart.
- **Continue Shopping Button:** Conveniently navigates back to the plant catalog view.
- **Checkout Button:** Alerts user with a *"Coming Soon! Thank you for choosing Paradise Nursery."* message.

---

## Technologies Used

- **React 18** (Functional components, Hooks: `useState`, `useEffect`)
- **Redux Toolkit (`@reduxjs/toolkit`)** (Centralized state management with `createSlice`)
- **React-Redux** (`useSelector`, `useDispatch`, `Provider`)
- **Vite** (Next-generation frontend tooling and bundler)
- **HTML5 & CSS3** (Custom styling, responsive flexbox layout, media queries)

---

## Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Shravanin3/e-plantShopping.git
   cd e-plantShopping
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Run the development server:**
   ```bash
   npm run dev
   ```

4. **Build for production:**
   ```bash
   npm run build
   ```

---

## License

This project is licensed under the MIT License.
