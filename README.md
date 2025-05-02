<<<<<<< HEAD
## 🛒 Hakim Livs Webshop — Fullstack Project

This is a fullstack e-commerce application built for the client *Hakim* by a cross-functional student team using the **MERN stack** (MongoDB, Express.js, React, Node.js) following **Scrum methodology**.

### 🔧 Backend (Node.js + Express)

- **Framework**: Express.js (Node.js)
- **Database**: MongoDB (via Mongoose)
  - **Pros**: Flexible schema, fast prototyping, easy scaling
  - **Cons**: Less strict structure, potential for unvalidated data if not properly modeled
- **Key Features**:
  - JWT-based authentication with role-based access (`admin`, `user`)
  - RESTful API with endpoints for products, categories, users, and orders
  - Admin-restricted product management
  - Public and protected order flows
- **Challenges**: Schema validation, secure auth token handling, syncing test data during development
- **API Documentation**: Available live at `/api/` and in Postman JSON format

### 🎨 Frontend (Vanilla JavaScript + HTML/CSS)

- **Tech**: HTML5, CSS3, JavaScript (ES6+)
- **Architecture**:
  - Modular JavaScript with reusable helpers
  - JWT token stored in localStorage for auth
- **Key Features**:
  - Product browsing and filtering
  - Guest and authenticated checkout
  - Admin panel for product CRUD
  - Dynamic UI updates with Fetch API
- **Deployment**: Static hosting (e.g., GitHub Pages)
- Backend, frontend, and testing coordinated under 3 Product Owners
- Final handover includes code, API documentation, and live demo support

---

Would you like a more visual summary (e.g. diagram or badges) for this README?
=======
# Hakim Livs - Frontend Handover (Webshop-2025-FE-G1)

## ✨ Project Overview

This is the frontend of the Hakim Livs Webshop, built by Group 1 during the frontend sprint of 2025. The webshop allows customers to browse products, add them to the cart, and place orders. It also features an admin panel for managing products. The project supports both guest users and logged-in users, with enhanced functionality available for admins.

## 📚 Repository

Frontend GitHub repo: [Webshop-2025-FE-G1](https://github.com/mansi-fed24/Webshop-2025-FE-G1.git)

## 📚 Setup & Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/mansi-fed24/Webshop-2025-FE-G1.git
   ```
2. Open `index.html` with Live Server or any local server environment.
3. No external packages are needed, the project uses vanilla HTML/CSS/JavaScript.

## 🌐 Technologies Used

- **HTML5**
- **CSS3**
- **JavaScript (ES6+)**
- **Fetch API**
- **JWT (via localStorage)**

Useful Links:

- [JavaScript Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [Vanilla JS JWT Handling](https://jwt.io/introduction)

## 🗃️ Code Structure & Key Files

```
├── index.html               # Homepage
├── products.html            # Product overview page
├── cart.html                # Cart page
├── checkout.html            # Checkout page
├── login.html               # User login
├── admin-product.html       # Admin dashboard for product management
├── js/
│   ├── index.js             # Loads products on homepage
│   ├── products.js          # Loads all products on product page
│   ├── cart.js              # Handles cart rendering
│   ├── checkout.js          # Handles form and order submission
│   ├── login.js             # Handles user login
│   ├── admin-product.js     # Admin product overview and delete/edit
│   ├── admin-addproduct.js  # Handles product addition
│   └── utils/
│       ├── cartFunctions.js # Shared cart functions
│       └── api.js           # Reusable helper functions like toggleAdminLink
├── css/                     # Contains CSS files for each page
```

## 🔧 Feature Breakdown

### 🔐 Admin Panel
- Developed a secure admin interface accessible only to authenticated admins.
- Implemented functionalities to **add, edit, and delete products**.

**Files involved:**
- `admin-product.html`
- `admin-product.css`
- `admin-product.js`
- `admin-addproduct.js`

### 👤 Authentication & User Management
- Created a login system allowing users to authenticate and access personalized features.
- Displayed logged-in user info across pages (e.g., `Inloggad som:`).

**Files involved:**
- `login.html`
- `login.css`
- `login.js`

### 🛍️ Shopping Cart & Checkout
- Users can add, view, and manage products in their cart.
- Checkout includes form validation and order confirmation.

**Files involved:**
- `cart.js`, `checkout.js`
- `cart.html`, `checkout.html`

### 🏠 Homepage & Product Display
- Dynamically loaded products on homepage and product listing pages.
- Enabled seamless navigation and product interaction.

**Files involved:**
- `index.js`, `products.js`
- `index.html`, `products.html`

### 🎨 Styling
- Applied consistent styling across all pages for better UI/UX.

**Files involved:**
- `admin-product.css`, `login.css`, `cart.css`, `checkout.css`, `index.css`, `products.css`

## ⚖️ Admin Functionality

- Admin users can:
  - Access the `admin-product.html` page.
  - Add, edit, and delete products.
  - Only visible if user is admin (via localStorage flag `isAdmin`).

## ⚡ Reusable Helper Functions

**Located in**: `utils/cartFunctions.js`, `utils/api.js`

### `updateDOMWithCartData()`
- Syncs cart content between localStorage and the UI.

### `getAggregatedCart()`
- Returns full cart details with quantities, subtotals, and total.

### `toggleAdminLink()`
- Shows/hides the admin panel link based on login status and user role.

## ⚠ Points of Improvement

- Centralize form validation for reuse across multiple pages.
- Refactor admin page to use modular components.
- Enhance user feedback messages and error handling.
- Improve responsive styling across all viewports.
- Extract common header/footer components.

## 📊 Deployment Instructions (Frontend)

1. Host HTML/CSS/JS files on any static hosting platform (e.g., GitHub Pages, Netlify, Vercel).
2. Ensure CORS is properly enabled on the backend.
3. Update base URL if backend endpoint changes.

## 🌐 Env Variables (if needed)

None used for frontend in local setup.

## 🚀 How to Start Locally

1. Clone the repo.
2. Use VS Code + Live Server or any other server to open `index.html`.
3. Log in using:
   - Admin credentials to access admin panel.
   - user register and login 
   - Or continue as guest.

## 📅 Final Note

This frontend is designed to be fully functional and scalable. The code is documented and structured in a way that makes it easy to hand over to the next group or developer. For any questions, refer to this README or reach out through the GitHub issues section.
>>>>>>> 281b15b (initial commit)
