
# Dot Glasses E-Commerce React Project

## Overview

This is a simple React-based e-commerce project for an eyewear store called **Dot Glasses**.
It allows users to:

* Browse products
* Add products to a cart with quantity management
* View cart items with images and quantities
* Checkout by submitting their details
* See a thank-you page with a detailed order summary including product images

---

## Features

* **Product Page:** Displays products with an "Add to Cart" button and quantity management.
* **Cart Page:** Shows selected products with images, quantity increment (+) button, and total price.
* **Checkout Page:** Collects user info (name, address, contact, discount), shows cart summary, and calculates total price.
* **Thank You Page:** Displays customer details, all ordered products with images, quantities, and subtotal price, plus the total order amount.
* Persistent cart and order data stored in `localStorage`.
* Responsive and clean UI layout using basic CSS and React hooks.

---

## Project Structure

```
src/
 ├── components/
 │    └── ProductCard.js          # Card component for each product on the product page
 ├── data/
 │    └── products.js             # Product data with id, name, price, image, etc.
 ├── pages/
 │    ├── ProductPage.js          # Lists all products
 │    ├── CartPage.js             # Shows cart contents and quantity control
 │    ├── CheckoutPage.js         # Form and order summary
 │    └── ThankYouPage.js         # Order confirmation with product images
 ├── App.js                      # React Router setup and routes
 └── index.js                    # React DOM rendering
```

---

## How to Run

1. Clone the repo:

```bash
git clone <your-repo-url>
cd dot-glasses
```

2. Install dependencies:

```bash
npm install
```

3. Run the development server:

```bash
npm start
```

4. Open [http://localhost:3000](http://localhost:3000) to view in the browser.

---

## Usage

* On the **Product Page**, click **Add to Cart** for your chosen glasses. Quantity will increase if you add the same product multiple times.
* Click **Go to Cart** to view your selections. Increase quantity using the `+` button.
* Proceed to **Checkout**, fill in your details, and place the order.
* See the **Thank You Page** with your order summary including images and total cost.

---

## Important Notes

* Make sure product images are correctly referenced in your `products.js` file (relative URLs or hosted images).
* The cart and order data are saved in the browser’s `localStorage`. Clearing browser data will reset the cart.
* Discount code input is present but does not apply any discount logic yet (can be extended).
* After placing the order, the cart is cleared automatically.

---

## Future Improvements

* Add discount code validation and price adjustment.
* Implement backend API for real orders and payment processing.
* Add product removal from cart functionality.
* Improve styling and responsiveness with frameworks like Bootstrap or TailwindCSS.
* Add user authentication and order history.

