# 🛒 MERN Ecommerce: A Seamless Shopping Experience Powered by the MERN Stack, Redux Toolkit, and Material UI

### Also try -> [https://mernchat.in](https://mernchat.in)
### ```Note✨: I have another amazing project on``` [End-to-End Encrypted Chat Application](https://github.com/Balaganesh1122/mern-chat) ```using Next.js, Prisma, PostgreSQL, Express, Socket.io.```

---

**MERN Ecommerce** is a **full-stack e-commerce web application** designed to provide a smooth, modern, and interactive shopping experience.  
Built using the **MERN Stack (MongoDB, Express.js, React.js, Node.js)**, it leverages **Redux Toolkit** for efficient global state management and **Material UI** for a polished, responsive, and accessible interface.  

This project includes complete **user** and **admin** functionality — from browsing and ordering products to managing inventory and orders — representing a real-world, production-ready e-commerce system.

---

## 📸 Screenshots

![ecommerce-homepage](https://github.com/Balaganesh1122/mern-ecommerce/blob/main/frontend/src/assets/images/front.png?raw=true)
![ecommerce-banner](https://github.com/Balaganesh1122/mern-ecommerce/blob/main/frontend/src/assets/images/banner3.jpg?raw=true)

---

## 🚀 Features

### 👤 **User Features**
- **Product Reviews**
  - Users can write, edit, and delete reviews.
  - Real-time updates for product ratings and review stats.
- **Wishlist**
  - Add or remove favorite products and annotate with personal notes.
- **Shopping Cart**
  - Add multiple items, update quantities, and calculate total costs dynamically.
- **Order Management**
  - Place new orders, view order history, and track delivery status.
- **Profile Management**
  - Manage username, email, and multiple shipping addresses.
  - Update account details easily through a user-friendly interface.

---

### 🧑‍💼 **Admin Features**
- **Product Management**
  - Add, edit, delete, and soft-delete products.
  - Manage stock, pricing, and product attributes.
- **Order Management**
  - View and manage all customer orders.
  - Update order statuses and view order details.
- **Dashboard Insights**
  - Monitor product listings, sales performance, and user activities.

---

### 🔒 **Security & Authentication**
- **Secure Authentication Flow**
  - Login, Signup, Logout, OTP verification, and Password Reset.
  - JWT-based session management for secure API access.
- **Encrypted Credentials**
  - Passwords are encrypted using `bcrypt` before storing in MongoDB.
- **Authorization Layers**
  - Admin-only protected routes for critical operations.
- **Error Handling**
  - Comprehensive validation and custom error middleware for reliability.

---

### ⚙️ **Architecture and Scalability**
- Modular folder structure for maintainability.
- Follows MVC design pattern (Model-View-Controller).
- RESTful API endpoints for client-server communication.
- Scalable backend with MongoDB and Node.js, easily extendable for large datasets.
- Built for performance and growth using optimized queries and efficient state handling.

---

## 🧰 Tech Stack

| Category | Technologies Used |
|-----------|------------------|
| **Frontend** | React.js, Redux Toolkit, Material UI, Axios |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB (Mongoose ORM) |
| **Authentication** | JSON Web Token (JWT), bcrypt.js |
| **Email Services** | Nodemailer (for OTP and password resets) |
| **Dev Tools** | Nodemon, ESLint, Docker (optional) |

---

## 🛠️ Project Setup

### **Prerequisites**
- Node.js (v21.1.0 or later)
- MongoDB installed and running locally
- Git (to clone repository)

---

### **Clone the Repository**

```bash
git clone https://github.com/Balaganesh1122/mern-ecommerce.git

### **Navigate to the Project Directory**

cd mern-ecommerce

###**Install Dependencies**
### **Frontend**
cd frontend
npm install

### **Backend**
cd backend
npm install


### **Environment Configuration**
### **Backend (.env file)**
# Database connection
MONGO_URI="mongodb://localhost:27017/mern_ecommerce"

# Frontend URL
ORIGIN="http://localhost:3000"

# Email credentials for sending password resets and OTPs
EMAIL="your-email@example.com"
PASSWORD="your-email-password"

# Token and cookie expiration settings
LOGIN_TOKEN_EXPIRATION="30d"
OTP_EXPIRATION_TIME="120000"
PASSWORD_RESET_TOKEN_EXPIRATION="2m"
COOKIE_EXPIRATION_DAYS="30"

# Secret key for JWT
SECRET_KEY="your-secret-key"

# Environment
PRODUCTION="false"

### **Data Seeding**
cd backend
npm run seed

### **Folder Structure**
mern-ecommerce/
│
├── backend/
│   ├── config/         # Database and environment setup
│   ├── controllers/    # Business logic and route handling
│   ├── models/         # Mongoose schemas (User, Product, Order)
│   ├── routes/         # API routes for users, products, orders
│   ├── middleware/     # Auth and error handling middleware
│   ├── utils/          # Helper utilities (JWT, Email)
│   └── server.js       # Main entry point
│
├── frontend/
│   ├── src/
│   │   ├── components/ # React components
│   │   ├── pages/      # React pages (Home, Cart, Product, etc.)
│   │   ├── redux/      # Redux slices for state management
│   │   ├── assets/     # Images and static files
│   │   └── utils/      # Utility functions
│   └── package.json
│
└── README.md


