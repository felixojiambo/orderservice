# E-Commerce Backend API

This Express and TypeScript project manages shopping cart and order functionalities. It includes endpoints for creating, updating, retrieving, and deleting cart items and orders. Middleware handles authentication and request validation.

## Usage

### Endpoints

#### Cart

- **Create**: `/cart` (POST)
- **Get**: `/cart` (GET)
- **Update**: `/cart/:id` (PATCH)
- **Delete**: `/cart/:id` (DELETE)

#### Order

- **Create**: `/order` (POST)
- **Get All**: `/order` (GET)
- **Get by ID**: `/order/:id` (GET)
- **Delete**: `/order/:id` (DELETE)

## Error Handling

The API returns appropriate HTTP status codes and error messages for various error conditions.

## Dependencies

- **express**: Web framework for Node.js.
- **typescript**: TypeScript language.
- **jwt**: Authentication.
- **class-validator**: Request validation.
