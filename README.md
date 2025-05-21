# 🛒 E-Commerce Backend API

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-4DB33D?style=for-the-badge&logo=mongodb&logoColor=white)
![License](https://img.shields.io/github/license/mostafamoknaa/MEAN-Project?style=for-the-badge)

A fully-featured e-commerce backend built with **Node.js**, **Express.js**, and **MongoDB Atlas**. This project handles user authentication, product listings, orders, payments, reviews, cart and wishlist management, and admin/seller functionalities.

---

## 📦 Features

### 👤 User Management
- Registration & login (Email, Phone, Social Media)
- Profile update (name, address, payment details)
- User roles (Customer, Seller, Admin)
- Wishlist & Order History
- Product Reviews & Ratings

### 🛍️ Product Management
- Categories and product listings
- Product images, descriptions, prices, and stock tracking
- Search and filter by name, price, category

### 🛒 Shopping Cart & Checkout
- Add/remove/edit items in cart
- Guest checkout option
- Multiple payment methods (Credit Card, Stripe, Cash on Delivery)
- Promo code and discount application

### 📦 Order Management
- Place orders & track statuses
- User order history
- Admin/seller order processing

### 💳 Payment Integration
- Stripe payment gateway
- Card saving and auto-fill

### 🔧 Admin Panel
- Manage users, products, categories, and orders
- Configure promo codes
- Content management (banners, homepage)

### 🛍️ Seller Features
- Seller account creation
- Manage product listings and inventory

---

## 📁 API Endpoints

### 👤 User Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/signup` | Register user |
| POST   | `/login` | Login user |
| GET    | `/verify/:email` | Email verification |
| GET    | `/getuserinfo` | Get profile (auth) |
| PUT    | `/updateuserinfo` | Update profile (auth) |
| DELETE | `/deleteuserinfo` | Delete account (auth) |

### 🔧 Admin Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | `/users` | Get all users (admin) |
| GET    | `/users/:id` | Get user by ID |
| POST   | `/users` | Create user (admin) |
| PUT    | `/users/:id` | Update user (admin) |
| DELETE | `/users/:id` | Delete user (admin) |

### 🛍️ Product Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/product` | Create product (seller) |
| GET    | `/product` | Get seller’s products (auth) |
| GET    | `/allproduct` | Get all products (public) |
| PUT    | `/product/:id` | Update product (seller) |
| DELETE | `/product/:id` | Delete product (seller) |

### 📦 Order Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/order` | Place order (auth) |
| GET    | `/getallorders` | Get all orders (auth) |
| GET    | `/getAllOrdersofUser` | User's orders (auth) |
| PUT    | `/order/:id` | Update order (auth) |
| DELETE | `/order/:id` | Delete order (auth) |

### ❤️ Wishlist Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/addtowishlist` | Add to wishlist (auth) |
| DELETE | `/deletefromwishlist/:id` | Remove from wishlist (auth) |

### 🛒 Cart Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | `/getusercart/:userid` | Get user cart |
| POST   | `/addtocart` | Add item to cart |
| PUT    | `/updatecartquantity` | Update item quantity |
| DELETE | `/deletefromcart/:userid` | Remove item from cart |
| POST   | `/gustuser` | Guest checkout |
| POST   | `/processpayment/:userid` | Process payment |
| POST   | `/applypromocode/:userid` | Apply promo code |

### 🛍️ Seller Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/createseller` | Register seller (auth) |

### ⭐ Review Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/review` | Create review (auth) |
| GET    | `/review` | Get user reviews (auth) |
| GET    | `/review/:id` | Get product reviews |
| GET    | `/adminreview` | Admin get all reviews |
| DELETE | `/review/:id` | Delete review (admin) |

### 🏷️ Promo Code Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST   | `/createpromocode` | Create promo code |
| DELETE | `/deletepromocode/:id` | Delete promo code |

---

## ⚙️ Installation & Setup

### 📋 Prerequisites
- Node.js installed
- MongoDB Atlas account


