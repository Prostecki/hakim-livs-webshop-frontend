# 🛒 Hakim Livs Webshop — Frontend (2025)

**Hakim Livs Webshop** is a fully functional e-commerce application built using the **MERN stack** (MongoDB, Express.js, React, Node.js) as part of a collaborative student project. This repository contains the **frontend** implementation using **Vanilla JavaScript, HTML, and CSS**.

> 📦 **Backend is maintained in a separate repository:**  
> 🔗 [View the Backend Repository](https://github.com/Prostecki/hakim-livs-webshop)

---

## 🎯 Project Goals

- Practice real-world development using the **Scrum** methodology  
- Build a scalable and responsive online store  
- Implement role-based user functionality: **guest**, **authenticated user**, and **admin**  
- Support a complete product flow: browsing, cart management, checkout, and order confirmation

---

## 🌐 Technologies Used

### Frontend
- **HTML5**
- **CSS3**
- **JavaScript (ES6+)**
- **Fetch API**
- **JWT-based authentication** (handled via `localStorage`)

---

## 🚀 Getting Started

### 1. Clone the repository:
```bash
git clone https://github.com/mansi-fed24/Webshop-2025-FE-G1.git
```

### 2. Launch locally:
- Open `index.html` using [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) in VS Code  
- No additional dependencies are required

---

## 🗂 Project Structure

```
├── index.html               # Homepage
├── products.html            # Product overview
├── cart.html                # Shopping cart
├── checkout.html            # Checkout form
├── login.html               # User login
├── admin-product.html       # Admin panel
├── js/
│   ├── index.js
│   ├── products.js
│   ├── cart.js
│   ├── checkout.js
│   ├── login.js
│   ├── admin-product.js
│   ├── admin-addproduct.js
│   └── utils/
│       ├── cartFunctions.js
│       └── api.js
├── css/
│   ├── index.css
│   ├── products.css
│   ├── cart.css
│   ├── checkout.css
│   ├── login.css
│   ├── admin-product.css
```

---

## 🔑 Features

### 🧾 General Functionality
- View and filter products
- Add products to cart as a guest or logged-in user
- Persist cart across sessions

### 🔐 Authentication & Roles
- Login via JWT tokens
- Admins have access to a separate panel for managing products
- Auth status and roles are stored in `localStorage`

### 🛍️ Shopping Cart & Checkout
- Update quantities and remove items
- Validate and submit checkout form
- Display confirmation messages after order placement

### ⚙️ Admin Panel
- Restricted to users with `isAdmin` flag
- Add/edit/delete products
- Accessible only when logged in as admin

---

## ⚡ Reusable Utilities

| Function | Description |
|----------|-------------|
| `updateDOMWithCartData()` | Synchronizes cart data with UI |
| `getAggregatedCart()`     | Calculates totals and quantities |
| `toggleAdminLink()`       | Shows/hides admin nav links |

---

## 📦 Deployment

You can host this frontend on any static hosting service such as:
- **GitHub Pages**
- **Netlify**
- **Vercel**

> ⚠ Ensure CORS settings are correctly configured on the backend for cross-origin API requests.

---

## 🧪 Recommendations for Improvement

- Centralize form validation logic  
- Refactor admin panel into components or modules  
- Improve responsiveness on smaller viewports  
- Add user feedback and error messages  
- Abstract shared components like headers/footers

---

## 👥 Team Notes

- Developed as part of a frontend sprint by Group 1 (2025)
- Collaborated with separate backend and testing teams
- Final handoff includes code, API docs, and demo instructions
