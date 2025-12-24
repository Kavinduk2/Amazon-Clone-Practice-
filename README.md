# Amazon E-Commerce Clone

A frontend clone of the Amazon e-commerce platform. This project mimics the core user interface and interaction flows of Amazon, including product browsing, cart management, checkout flows, and order tracking. It uses vanilla JavaScript to generate dynamic product grids and manage cart state.

## 🚀 Features

* **Dynamic Product Listing:** The homepage programmatically generates product cards (images, ratings, prices) using JavaScript loops.
* **Interactive Cart System:**
    * Users can select quantities (1-10) and add items to the cart.
    * The cart counter in the header updates instantly upon addition.
    * A "Successfully added" confirmation message appears and fades out automatically after 1.5 seconds.
* **Responsive UI:** All pages include viewport meta tags to ensure the layout adapts to mobile and tablet screens.
* **Multi-Page Navigation:**
    * **Home:** Product browsing and search bar interface.
    * **Checkout:** Order review, delivery date selection, and payment summary (Subtotal, Shipping, Tax, Total).
    * **Orders:** History of past purchases with "Buy it again" and "Track package" options.
    * **Tracking:** Visual progress bar showing delivery status (Preparing -> Shipped -> Delivered).

## 🛠 Technologies Used

* **HTML5:** Semantic structure for product grids, headers, and forms.
* **CSS3:** (Linked files) Styling for Flexbox/Grid layouts, shared navigation bars, and responsive design.
* **Vanilla JavaScript (ES6+):** Handles DOM manipulation, event listeners, and data rendering without external frameworks.

## 📂 Project Structure

| File | Description |
| :--- | :--- |
| `amazon.html` | The main landing page. Contains the header and the empty container for the product grid. |
| `amazon.js` | The core script. It iterates through product data to generate HTML, handles "Add to Cart" clicks, and updates the cart quantity UI. |
| `checkout.html` | The shopping cart page. Displays selected items, delivery options (dates/prices), and the final order summary. |
| `orders.html` | Displays a history of placed orders with Order IDs, dates, and total costs. |
| `tracking.html` | A visual interface for tracking the delivery status of a specific package. |

## ⚙️ How to Run

1.  **Download the Code:** Ensure all HTML files and the `amazon.js` file are in the root directory.
2.  **Verify Data Files:** Ensure you have the `data/` folder containing `cart.js` and `products.js`, as these are referenced by `amazon.html` to load the initial data.
3.  **Verify Images:** Ensure the `images/` directory is populated with the necessary icons and product images referenced in the HTML/JS.
4.  **Launch:** Open `amazon.html` in any modern web browser (Chrome, Firefox, Edge).

## 🚧 Current Status & Future Improvements

* **Dynamic Homepage:** The homepage fully utilizes JavaScript to render products.
* **Static Checkout/Orders:** Currently, `checkout.html` and `orders.html` utilize hardcoded HTML for layout demonstration.
    * *To-Do:* Refactor `checkout.html` to generate cart items dynamically based on the `cart` array.
    * *To-Do:* Implement actual calculation logic for the "Order Summary" in the checkout.
