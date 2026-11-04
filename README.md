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

<img width="1086" height="1012" alt="image" src="https://github.com/user-attachments/assets/1b16008f-d57a-40c9-8b75-bc936059dfbc" />


### 02. Create Product

<img width="1085" height="1013" alt="image" src="https://github.com/user-attachments/assets/35fe2aa3-130c-494d-8238-85e74cdc1e37" />


### 03. Product Validation

<img width="1086" height="938" alt="image" src="https://github.com/user-attachments/assets/b3147437-5289-485e-9305-0392f019972f" />


### 04. Filtering, Sorting & Pagination

<img width="1076" height="1005" alt="image" src="https://github.com/user-attachments/assets/01ec12a7-d5a7-462b-85a4-d82e35c42c98" />


### 05. Retrieve & Update Product

<img width="1095" height="935" alt="image" src="https://github.com/user-attachments/assets/e35f2a60-971c-4fbd-8a28-18676d21a5f3" />


### 06. Delete Product

<img width="1088" height="800" alt="image" src="https://github.com/user-attachments/assets/71e1744f-d22a-490b-a856-c8c263e9f843" />


### 07. Stock Adjustment & Low-Stock Report

<img width="1098" height="997" alt="image" src="https://github.com/user-attachments/assets/74cdd72b-bc0a-44c4-bb14-df56b05a9f8f" />
<img width="1082" height="1002" alt="image" src="https://github.com/user-attachments/assets/8192d3a2-05e6-4113-89db-cad1e9b53551" />
<img width="1098" height="725" alt="image" src="https://github.com/user-attachments/assets/fe3c77af-bed7-45f4-bbf7-8f983d9e104a" />


### 08. Category-wise Inventory Summary
<img width="1082" height="775" alt="image" src="https://github.com/user-attachments/assets/98455991-aba1-40cb-9205-62d8d034b3aa" />

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
