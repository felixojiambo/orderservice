This project is an e-commerce backend API built with Express and TypeScript. It manages shopping cart and order functionalities, including creating, updating, retrieving, and deleting cart items and orders. It includes middleware for authentication and request validation to ensure secure and accurate data handling.

Table of Contents
Installation
Usage
Endpoints
Cart Endpoints
Order Endpoints
Error Handling
Dependencies
Contributing
Installation
Clone the repository:

bash
Copy code
git clone <repository_url>
cd <repository_directory>
Install dependencies:

bash
Copy code
npm install
Start the server:

bash
Copy code
npm start
Usage
Endpoints
Cart Endpoints
Create Cart
URL: /cart
Method: POST
Description: Creates a new cart item.
Request Body:
json
Copy code
{
  "productId": "number",
  "quantity": "number"
}
Responses:
200 OK: Cart item created successfully.
403 Forbidden: Authorization error.
404 Not Found: Validation errors or server error.
Get Cart
URL: /cart
Method: GET
Description: Retrieves the cart for the authenticated user.
Responses:
200 OK: Cart retrieved successfully.
Edit Cart
URL: /cart/:lineItemId
Method: PATCH
Description: Updates a cart item.
Request Body:
json
Copy code
{
  "qty": "number"
}
Responses:
200 OK: Cart item updated successfully.
Delete Cart
URL: /cart/:lineItemId
Method: DELETE
Description: Deletes a cart item.
Responses:
200 OK: Cart item deleted successfully.
Order Endpoints
Create Order
URL: /order
Method: POST
Description: Creates a new order.
Responses:
200 OK: Order created successfully.
Get Orders
URL: /order
Method: GET
Description: Retrieves all orders.
Responses:
200 OK: Orders retrieved successfully.
Get Order by ID
URL: /order/:id
Method: GET
Description: Retrieves an order by its ID.
Responses:
200 OK: Order retrieved successfully.
Delete Order
URL: /order/:id
Method: DELETE
Description: Deletes an order by its ID.
Responses:
200 OK: Order deleted successfully.
Error Handling
The API returns appropriate HTTP status codes and error messages for various error conditions:

403 Forbidden: Returned when the user is not authorized.
404 Not Found: Returned when validation fails or a resource is not found.
500 Internal Server Error: Returned when an unexpected server error occurs.
Dependencies
express: Web framework for Node.js.
typescript: TypeScript language.
class-validator: Used for validating class instances.
jwt: Used for authentication.
Contributing
Feel free to submit issues or pull requests if you have suggestions for improvements or find any bugs.
