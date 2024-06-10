# E-commerce Application API

This project involves developing a RESTful API for a simple e-commerce application . The API includes basic CRUD operations for managing products. The API is designed to be consumed by a frontend application using Axios or the Fetch API.

<br/>

## Features

- CRUD operations for products (Create, Read, Update, Delete)
- JSON response format for easy integration with frontend applications

<br/>


## Utility Functions

- __Input Validation__: Validates user input for product management to ensure data integrity.
- __Error Handling__: Standardized error responses for invalid requests.
- __Database Connection__: Manages the connection to the database for storing and retrieving data.

<br/>

## API Reference

#### __Create Product Endpoint__: Creates a new product in the system.

```http
POST /api/products
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `name`| `string` | **Required**. The name of the product.|
| `description`| `string` | **Optional**. A description of the product.|        
| `price`| `float` | **Required**. The price of the product.|
| `stock`| `integer` | **Required**. The stock quantity of the product.|

#### __Get All Products Endpoint__: Retrieves a list of all products.

```http
GET /api/products
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |


#### __Get Product by ID Endpoint__: Retrieves details of a specific product by ID.

```http
GET /api/products/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id`| `integer` | **Required**. The ID of the product.|


#### __Update Product Endpoint__: Updates the details of a specific product.

```http
PUT /api/products/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id`| `integer` | **Required**. The ID of the product.|
| `name`| `string` | **Optional**. The name of the product.|
| `description`| `string` | **Optional**. A description of the product.|        
| `price`| `float` | **Optional**. The price of the product.|
| `stock`| `integer` | **Optional**. The stock quantity of the product.|


#### __Delete Product Endpoint__: Deletes a specific product from the system.

```http
DELETE /api/products/{id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `id`| `integer` | **Required**. The ID of the product.|

<br/>

## Support

For any questions, issues, or feature requests, please contact slazyslother@gmail.com

