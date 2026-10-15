# 🛒 ShopKart — Full-Stack E-Commerce Platform

ShopKart is a full-stack e-commerce web application built with the MERN stack. It provides a complete shopping experience, including customer authentication, product discovery, wishlist management, shopping cart functionality, checkout, and order tracking.

The application integrates **Razorpay Test Mode** for payment testing and uses a REST API to connect the React frontend with the Node.js backend.

## ✨ Features

### 🔐 Authentication
- Customer registration and login
- Secure password hashing with bcrypt
- JWT-based authentication
- Protected routes and user profile retrieval
- Logout and password change functionality

### 🛍️ Product Catalogue
- Browse products and view product details
- Search products by keyword
- Filter products by category
- Sort products by price
- Display product prices and stock availability

### ❤️ Wishlist
- Add and remove products from the wishlist
- View saved products
- Move wishlist items directly to the cart
- Display wishlist item counts

### 🛒 Shopping Cart
- Add products to the cart
- Increase or decrease item quantities
- Remove individual items
- Calculate subtotals automatically
- Validate available stock

### 💳 Checkout and Payments
- Collect and validate shipping information
- Create orders through the backend
- Integrate Razorpay Checkout in test mode
- Verify payment signatures on the server
- Update order status after payment verification
- Clear the cart after successful payment processing

### 📦 Order Management
- View order history
- View individual order details
- Track order status through a visual timeline

## 🧰 Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | React 19, Vite |
| Styling | Tailwind CSS v4 |
| Routing | React Router DOM |
| HTTP Client | Axios |
| Backend | Node.js, Express.js |
| Database | MongoDB, Mongoose |
| Authentication | JWT, bcrypt, HTTP-only cookies |
| Payment Gateway | Razorpay |
| Version Control | Git, GitHub |

## 🏗️ Project Architecture

ShopKart follows a client-server architecture.

- **Frontend:** Provides the user interface and communicates with the backend through HTTP requests.
- **Backend:** Handles authentication, product operations, cart and wishlist management, order creation, and payment verification.
- **Database:** Stores customer information, products, and orders.
- **Payment Gateway:** Razorpay Checkout handles the payment interface, while the backend verifies payment signatures.

## 📂 Project Structure

```text
web-dev-viva/
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── index.js
│   ├── package.json
│   └── .env.example
│
├── shopkart-frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── index.css
│   ├── package.json
│   └── vite.config.js
│
├── .gitignore
└── README.md
```

## ⚙️ Prerequisites

Install the following before running the project:

- [Node.js](https://nodejs.org/) — preferably a supported LTS version
- npm, included with Node.js
- [Git](https://git-scm.com/downloads/)
- MongoDB locally or a MongoDB Atlas connection, if required by your configuration
- A Razorpay account with Test Mode API credentials for payment testing

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/anilkavya310107-cpu/web-dev-viva.git
cd web-dev-viva
```

### 2. Configure the backend

Open a terminal in the project root and run:

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory by copying the example file.

**Windows PowerShell:**

```powershell
Copy-Item .env.example .env
```

Update `backend/.env` with your own configuration:

```env
