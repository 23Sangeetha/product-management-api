# Product Management API – Postman Collection

## Overview

This project is a **Product Management API testing collection** created using **Postman**. It demonstrates basic CRUD operations using a Product API.

The collection contains five API requests:

- List all products
- Create a new product
- Get a product
- Update an existing product
- Delete a product

---

## Collection Flow

```text
List Products
      ↓
Create Product
      ↓
Get Product
      ↓
Update Product
      ↓
Delete Product
```

---

# API Requests

## 1. List Products

**Method:** `GET`

```text
GET {{productBaseUrl}}/products
```

This request retrieves the list of all available products.

---

## 2. Create Product

**Method:** `POST`

```text
POST {{productBaseUrl}}/products
```

### Request Body

```json
{
  "name": "Samsung Galaxy S25",
  "price": 74999,
  "category": "Electronics",
  "stock": 20
}
```

This request creates a new product.

---

## 3. Get Product

**Method:** `GET`

```text
GET {{productBaseUrl}}/products/{{productId}}
```

This request retrieves the details of a specific product using its product ID.

---

## 4. Update Product

**Method:** `PUT`

```text
PUT {{productBaseUrl}}/products/{{productId}}
```

### Request Body

```json
{
  "name": "Samsung Galaxy S25 Ultra",
  "price": 89999,
  "category": "Premium Electronics",
  "stock": 15
}
```

This request updates the details of an existing product.

---

## 5. Delete Product

**Method:** `DELETE`

```text
DELETE {{productBaseUrl}}/products/{{productId}}
```

This request deletes the selected product.

---

## HTTP Methods Used

| Method | Operation |
|---|---|
| `GET` | List all products and get a specific product |
| `POST` | Create a new product |
| `PUT` | Update an existing product |
| `DELETE` | Delete a product |

---

## Tools Used

- Postman
- MockAPI
- GitHub

---

## Concepts Covered

- REST API
- CRUD Operations
- HTTP Methods
- GET, POST, PUT, and DELETE
- API Testing
- JSON Request and Response

---

## How to Run

Run the five requests in the following order:

```text
->List Products
->Create Product
-> Get Product
->Update Product
->Delete Product
```

---

## Author

**Sangeetha L**