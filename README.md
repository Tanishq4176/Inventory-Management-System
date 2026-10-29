<div align="center">

# 📦 Inventory Management System

### A RESTful API for Efficient Inventory Management

Built with Node.js, Express.js, MongoDB and Mongoose.

<br>

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=for-the-badge&logo=mongoose&logoColor=white)

</div>

---

## 📌 Overview

A backend application designed to manage product inventory, maintain stock levels, and generate inventory reports through RESTful APIs.

## ✨ Key Features

- **Product Management:** Create, retrieve, update and delete products.
- **Schema Validation:** Required fields, unique SKUs and numeric validation.
- **Inventory Queries:** Filtering, sorting and pagination.
- **Stock Adjustment:** Increase or decrease product quantities safely.
- **Low-Stock Alerts:** Identify products requiring replenishment.
- **Category Summary:** Generate inventory reports using MongoDB aggregation.
- **Error Handling:** Centralized handling of invalid requests and database errors.

## 🛠️ Tech Stack

| Technology | Purpose |
|:---|:---|
| Node.js | JavaScript runtime |
| Express.js | REST API development |
| MongoDB | Database |
| Mongoose | Schema modelling and validation |
| dotenv | Environment configuration |
| Postman | API testing |

## 🚀 Getting Started

**1. Clone the repository**

```bash
git clone https://github.com/HarshKamboj25/Inventory-Management-System.git
cd Inventory-Management-System
```

**2. Install dependencies**

```bash
npm install
```

**3. Configure environment variables**

Create a `.env` file in the project root:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
```

Replace the placeholder with your MongoDB connection string.

**4. Start the server**

```bash
node server.js
```

The API runs at `http://localhost:5000` by default.

## 🔗 API Endpoints

| Method | Endpoint | Description |
|:---:|:---|:---|
| GET | `/` | API health check |
| POST | `/api/products` | Create a product |
| GET | `/api/products` | Get products with query options |
| GET | `/api/products/:id` | Get a product by ID |
| PUT | `/api/products/:id` | Update product details |
| PATCH | `/api/products/:id/stock` | Adjust stock quantity |
| DELETE | `/api/products/:id` | Delete a product |
| GET | `/api/products/low-stock` | Retrieve low-stock products |
| GET | `/api/products/summary` | Category-wise inventory summary |

## 🔒 Security

- Keep database credentials in `.env`.
- Never commit actual credentials or secrets.
- Use `.env.example` to document required environment variables.

## 👨‍💻 Author

**Harsh Kamboj**

[GitHub Profile](https://github.com/HarshKamboj25) · [Project Repository](https://github.com/HarshKamboj25/Inventory-Management-System)

---

<div align="center">

**Built as part of the Web Development III assignment.**

</div>
