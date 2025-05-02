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
