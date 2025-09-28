# JavaScript Amazon Clone: Products & Cart Page
A responsive, client-side replica of an Amazon products page built with modern JavaScript. This project dynamically generates product listings from a data source, manages a shopping cart using local storage, and provides a seamless user experience for adding, updating, and viewing items.

Live Demo: Link to your deployed project <!-- TODO: Add your live demo link here -->

## Table of Contents
[Project Overview](#project-overview)

[Key Features](#key-features)

[Technologies Used](#technologies-used)

[Getting Started](#getting-started)

[Project Structure](#project-structure)

[How It Works](#how-it-works)

[Acknowledgements](#acknowledgements)


## Project Overview
This project was created to practice and demonstrate core JavaScript concepts, including DOM manipulation, modular design, and local state management. It simulates the front-end functionality of a basic e-commerce platform where users can browse products and manage their shopping cart. All data is handled on the client-side, making it a lightweight and fast-loading application.

## Key Features
+ **Dynamic Product Loading**: Products are generated dynamically from a JavaScript data object, making it easy to update the inventory.
+ **Interactive Shopping Cart**:
  + Add products to the cart directly from the product page.
  + View the total number of items in the cart updated in real-time in the header.
+ **Persistent Cart Data**: The shopping cart's state is saved to a `cart.js`, so items remain in the cart even after a page refresh or closing the browser.

## Technologies Used
+ **HTML5**: For the basic structure and semantic markup of the web pages.
+ **CSS3**: For styling, layout, and responsive design.
+ **Vanilla JavaScript (ES6+)**: For all the dynamic functionality, including DOM manipulation, event handling, and business logic.
+ **No frameworks or libraries were used** in this project to focus on core web technologies.

## Getting Started
To run this project locally, follow these simple steps:
**1. Clone the repository**:
git clone [https://github.com/jatinbalajisailada/javascript-amazon-products-page.git](https://github.com/jatinbalajisailada/javascript-amazon-products-page.git)

**2. Navigate to the project directory**:
cd javascript-amazon-products-page

**3. Open amazon.html in your web browser**:
  + You can simply double-click the amazon.html file in your file explorer.
  + **Recommended**: Use a live server extension (like "Live Server" in VS Code) to run the project. This helps prevent potential CORS issues with local file access.
    
That's it! You should now see the application running in your browser.

## Project Structure
The repository is organized as follows:
```
/
├── amazon.html             # The main products page
├── checkout.html           # The shopping cart/checkout page
├── data/
│   └── products.js         # Data module containing product information
│   └── cart.js             # Module for cart-related functions
├── images/                 # Contains all product and site images
├── scripts/
│   └── amazon.js           # Main script for the products page
│   └── checkout.js         # Script for the checkout page functionality
└── styles/
    └── main.css            # General styles for the entire site
    └── amazon.css          # Specific styles for the product grid
    └── checkout.css        # Styles for the checkout page
```
## How It Works
**1. Data Management**: The product list is stored in `data/products.js` as an array of objects.

**2. Product Rendering**: The `scripts/amazon.js` script imports the product data and dynamically creates the HTML for each product card, then injects it into the main grid on amazon.html.

**3. Cart Logic**: The `data/cart.js` module contains all the functions to manage the cart (addToCart, calculateCartQuantity, etc.). When a user adds an item, this module updates a cart array, which is then saved to localStorage.

## Acknowledgements
+ This project was inspired by the "JavaScript & HTML/CSS" course on SuperSimpleDev.
+ Product images and descriptions are for demonstrative purposes only.

