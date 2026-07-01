# 📦 Order Management Dashboard

A full-stack **Order Management Dashboard** built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js). This application allows users to manage customer orders, track order statuses, and view order statistics through a clean and responsive dashboard.

---

## 🚀 Features

- 📋 View all customer orders
- ➕ Add new orders
- 🔄 Refresh order list
- 🔍 Filter orders by status
- 📊 Dashboard summary cards
- 💾 MongoDB database integration
- 🌐 REST API with Express.js
- 📱 Responsive user interface
- ⚡ Real-time data fetching using Axios

---

## 🛠️ Tech Stack

### Frontend
- React.js
- Axios
- React Icons
- CSS3

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- CORS
- Dotenv

### Database
- MongoDB

---

## 📁 Project Structure

```
oms-dashboard/
│
|   backend/
|      ├── config/
|      │    └── db.js
|      ├── models/
|      │    └── Order.js
|      ├── routes/
|      │    └── orderRoutes.js
|      ├── controllers/
|      │    └── orderController.js
|      ├── scheduler/
|      │    └── orderScheduler.js
|      ├── server.js
|           └── package.json
│
├── frontend/
│   ├── public/
│   ├── src/
|   |  ├── components/
|   │    ├── Sidebar.js
|   │    ├── StatsCard.js
|   │    ├── OrdersTable.js
|   │    └── Filter.js
|   ├── pages/
|   │    └── Dashboard.js
|   |    └── Dashboard.css
|   ├── App.js
|   └── index.js
│
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/order-management-dashboard.git
```

### 2. Navigate to the project

```bash
cd order-management-dashboard
```

---

## Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the `backend` folder.

```env
MONGO_URI=mongodb://localhost:27017/orderDB
PORT=5000
```

Start the backend server:

```bash
npm start
```

Server runs on:

```
http://localhost:5000
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm start
```

Frontend runs on:

```
http://localhost:3000
```

---

## API Endpoints

### Get All Orders

```
GET /api/orders
```

### Create Order

```
POST /api/orders
```

Example Request

```json
{
  "customer": "Rishabh",
  "product": "Laptop",
  "quantity": 2,
  "amount": 85000,
  "paymentStatus": "PAID",
  "status": "PLACED"
}
```

---

## MongoDB Schema

```javascript
{
  customer: String,
  product: String,
  quantity: Number,
  amount: Number,
  paymentStatus: String,
  status: String,
  createdAt: Date
}
```

---

## Dashboard Overview

The dashboard includes:

- Total Orders
- Placed Orders
- Processing Orders
- Ready to Ship Orders
- Order List Table
- Refresh Orders
- Status Filter

---

## Future Improvements

- Edit Order
- Delete Order
- Authentication
- Search Orders
- Pagination
- Charts & Analytics
- Export to Excel/PDF
- Dark Mode
- Role-based Access

---

## Screenshots

Add screenshots of:

- Dashboard
- Orders Table
- MongoDB Collection
- API Response

---

## Author

**Rishabh Sharma**

GitHub: https://github.com/bhardawjrishabh452-stack

LinkedIn: www.linkedin.com/in/rishabh-sharma-25436521b

---

## License

This project is licensed under the MIT License.
