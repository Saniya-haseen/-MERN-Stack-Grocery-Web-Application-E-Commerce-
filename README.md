# 🛒 MERN Stack Grocery Web Application (E-Commerce)

A full-stack e-commerce platform for online grocery shopping, built with the MERN stack — MongoDB, Express.js, React.js, and Node.js.

> **B.Tech Project** | SRM University–AP | Computer Science and Engineering  
> Submitted by: S. Saniya Haseen, P AnuTejaswini, Devi Sree Honne.
> Guided by: Himanshu Mishra Sir, Asst. Professor, Dept. of CSE

---

## 📌 About the Project

This application replicates the physical grocery shopping experience online with added convenience, speed, and automation. It supports two primary roles — **Customers** and **Admins** — each with dedicated features and access control.

---

## ✨ Features

### 👤 Customer
- Register & login with secure JWT authentication
- Browse products by category (Fruits, Vegetables, Dairy, Beverages, Bakery)
- Filter by brand & price, search by name
- Real-time shopping cart with quantity & subtotal updates
- Checkout with address entry and PayPal payment integration
- View order history & track order status
- Leave product reviews and ratings

### 🔐 Admin
- Role-based secure login
- Add, edit, delete products with image uploads
- Monitor and update stock levels
- Manage and update order statuses (Pending → Shipped → Delivered)
- View and manage customer feedback

---

## 🛠️ Tech Stack

| Layer      | Technology                          |
|------------|--------------------------------------|
| Frontend   | React.js, Redux Toolkit, Tailwind CSS |
| Backend    | Node.js, Express.js                  |
| Database   | MongoDB, Mongoose                    |
| Auth       | JWT, bcrypt                          |
| Storage    | Cloudinary (image hosting)           |
| Payment    | PayPal Integration                   |

---

## 📁 Folder Structure

```
e-commerce/
├── client/               # React frontend
│   ├── public/
│   ├── src/
│   ├── tailwind.config.js
│   └── vite.config.js
└── server/               # Node.js backend
    ├── controllers/
    ├── helpers/
    ├── models/
    └── routes/
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v16.x or newer)
- npm
- MongoDB (local or Atlas)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Saniya-haseen/-MERN-Stack-Grocery-Web-Application-E-Commerce-.git
   cd E-Commerce
   ```

2. **Install dependencies**

   For the client:
   ```bash
   cd client
   npm install
   ```

   For the server:
   ```bash
   cd server
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the `server` directory:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloud_name
   CLOUDINARY_API_KEY=your_api_key
   CLOUDINARY_API_SECRET=your_api_secret
   PAYPAL_CLIENT_ID=your_paypal_client_id
   ```

4. **Run the application**

   Frontend (in `/client`):
   ```bash
   npm run dev
   ```

   Backend (in `/server`):
   ```bash
   npm run dev
   ```

---

## 🔗 API Routes

| Route File          | Description                              |
|---------------------|------------------------------------------|
| `authroutes.js`     | User registration, login, session        |
| `product-routes.js` | Admin product management (CRUD)          |
| `order-routes.js`   | Place and track orders                   |
| `cart-routes.js`    | Cart item management                     |
| `review-routes.js`  | Product reviews by users                 |

All APIs follow RESTful conventions and communicate over HTTPS using JSON.

---

## 📽️ Demo Videos

- [Frontend Demo](https://drive.google.com/file/d/1Abm7wV8nZNfYMJIQhYGBHyMNh6ufUkP2/view?usp=drivesdk)
- [Backend Demo](https://drive.google.com/file/d/1lpipG7_fZmIT684HGu1ZLSzK68_SS0BT/view?usp=drivesdk)

---

## ⚠️ Known Issues

- Session may expire during active use (refresh token mechanism planned)
- PayPal pop-up may fail on Safari — use Chrome/Firefox
- Inventory sync may lag ~30 seconds under concurrent cart updates
- Bulk admin uploads limited to 50 products / 5MB per image

---

## 🔮 Future Enhancements

- Real-time GPS-based order tracking
- Progressive Web App (PWA) support
- AI-based product recommendations
- Voice search & chatbot support
- Multi-language support
- UPI / digital wallet payment options
- Loyalty & rewards program
- Automated low-stock alerts

---

## 🙏 Acknowledgements

Thanks to our mentor **Himanshu Mishra Sir** for his guidance, and to SRM University–AP for providing the resources and platform to complete this project.
