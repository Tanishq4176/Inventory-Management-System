 <div align="center">

# 📦 INVENTORY MANAGEMENT SYSTEM

### RESTful Inventory API | Smart Stock Management | Real-Time Reports

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=800&color=36BCF7&center=true&vCenter=true&width=650&lines=Manage+Products+Efficiently;Track+Inventory+with+REST+APIs;Monitor+Stock+Levels;Generate+Smart+Inventory+Reports" alt="Animated typing banner" />

<br/>

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=for-the-badge&logo=mongoose&logoColor=white)

<br/>

**A backend-powered solution for efficient product and inventory management.**

[Features](#-key-features) • [Tech Stack](#-tech-stack) • [API](#-api-endpoints) • [Testing](#-api-testing--screenshots) • [Setup](#-getting-started)

<br/>

<!-- Add your actual animated demo GIF at assets/inventory-demo.gif -->
<img src="assets/inventory-demo.gif" width="85%" alt="Inventory Management System animated demo"/>

<sub>⚡ Inventory management made structured, reliable and efficient.</sub>

</div>

---

## 📌 Overview

The **Inventory Management System** is a backend application built to simplify product management and inventory tracking through RESTful APIs.

It provides essential operations for managing products, maintaining stock levels, monitoring low-stock items, and generating category-wise inventory reports using MongoDB aggregation.

## ✨ Key Features

<table>
<tr>
<td width="50%">

### 📦 Product Management
Create, retrieve, update and delete products with structured API endpoints.

### 🛡️ Data Validation
Required-field checks, unique SKU constraints and numeric validation.

### 🔎 Advanced Inventory Queries
Filter, sort and paginate product records.

### 📊 Inventory Reports
Generate category-wise summaries using MongoDB aggregation.

</td>
<td width="50%">

### 🔄 Stock Management
Increase or decrease product quantities safely.

### 🚨 Low-Stock Alerts
Identify products that have reached or fallen below their reorder level.

### ⚙️ Centralized Error Handling
Handle validation, database and invalid-request errors consistently.

### 🔐 Environment Configuration
Keep database credentials and configuration in environment variables.

</td>
</tr>
</table>

## 🛠️ Tech Stack

| Technology | Usage |
|:---|:---|
| 🟢 Node.js | JavaScript runtime |
| ⚫ Express.js | REST API development |
| 🍃 MongoDB | NoSQL database |
| 🔴 Mongoose | Schema modelling and validation |
| 🔐 dotenv | Environment variable management |
| 🚀 Postman | API testing |

## 🏗️ Project Structure

```text
Inventory-Management-System/
│
├── middleware/
│   ├── errorHandler.js
│   └── validateProduct.js
│
├── models/
│   └── Product.js
│
├── routes/
│   └── productRoutes.js
│
├── .env.example
├── .gitignore
├── package.json
└── server.js
```

## 🔗 API Endpoints

| Method | Endpoint | Description |
|:---:|:---|:---|
| GET | `/` | API health check |
| POST | `/api/products` | Create a product |
| GET | `/api/products` | Retrieve products |
| GET | `/api/products/:id` | Get product by ID |
| PUT | `/api/products/:id` | Update product details |
| PATCH | `/api/products/:id/stock` | Adjust stock quantity |
| DELETE | `/api/products/:id` | Delete a product |
| GET | `/api/products/low-stock` | Retrieve low-stock products |
| GET | `/api/products/summary` | Category-wise inventory summary |

### 🔍 Query Parameters

The products endpoint supports:

- `category` : Filter products by category
- `minPrice` : Set minimum product price
- `maxPrice` : Set maximum product price
- `sort` : Select the sorting field
- `order` : Choose ascending or descending order
- `page` : Select the page number
- `limit` : Set the number of products per page

Example:

```http
GET /api/products?category=Electronics&sort=price&order=asc&page=1&limit=5
```

## 📸 API Testing & Screenshots

The following screenshots demonstrate the main API operations and their responses.

> Replace the image paths below with the actual screenshots committed to your repository.

### 01. Server & Database Connection

<img src="screenshots/01-server-running.png" width="90%" alt="Server running and database connected"/>

### 02. Create Product

<img src="screenshots/02-create-product.png" width="90%" alt="Successful product creation"/>

### 03. Product Validation

<img src="screenshots/03-product-validation.png" width="90%" alt="Product validation response"/>

### 04. Filtering, Sorting & Pagination

<img src="screenshots/04-filter-sort-pagination.png" width="90%" alt="Product filtering sorting and pagination"/>

### 05. Retrieve & Update Product

<img src="screenshots/05-get-and-update-product.png" width="90%" alt="Get and update product responses"/>

### 06. Delete Product

<img src="screenshots/06-delete-product.png" width="90%" alt="Product deletion response"/>

### 07. Stock Adjustment & Low-Stock Report

<img src="screenshots/07-stock-and-low-stock.png" width="90%" alt="Stock adjustment and low stock report"/>

### 08. Category-wise Inventory Summary

<img src="screenshots/08-category-summary.png" width="90%" alt="Category-wise inventory aggregation response"/>

## 🚀 Getting Started

Follow these steps to run the project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/HarshKamboj25/Inventory-Management-System.git

cd Inventory-Management-System
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
```

Replace the placeholder with your MongoDB connection string.

### 4. Start the Server

```bash
node server.js
```

The API will be available at:

```text
http://localhost:5000
```

## 🔒 Security & Best Practices

- Store database credentials in `.env`.
- Never commit actual credentials or secrets.
- Keep `.env` excluded through `.gitignore`.
- Use `.env.example` to document required configuration.
- Validate incoming data before database operations.
- Handle API errors through centralized middleware.

## 👩‍💻 Author

**Harsh Kamboj**

Backend Development | REST APIs | Database Management

---

<div align="center">

### ⭐ If you found this project interesting, consider giving it a star!

**Built with Node.js, Express.js & MongoDB**

<sub>Web Development III | Academic Project</sub>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:36BCF7,100:4776E6&height=100&section=footer" width="100%"/>

</div>
