# Simple Book API Postman Collection

This repository contains a Postman collection for the `Simple Book API`.

## Collection Contents

The collection includes the following API requests:

- `Status` - GET `/status`
- `List of Book` - GET `/books?type=fiction&limit=2`
- `Single Book` - GET `/books/:ID`
- `API Authentication` - POST `/api-clients/`
- `Submit an order` - POST `/orders`
- `Get all orders` - GET `/orders`
- `Update an order` - PATCH `/orders/:orderId`
- `Delete an order` - DELETE `/orders/:orderId`

## Environment Variables

The collection uses the following variables:

- `{{url}}` - Base API URL
- `{{token}}` - Bearer token for authenticated requests

Default values stored in the collection:

- `url`: `https://simple-books-api.glitch.me`

## Usage

1. Open Postman.
2. Import `Simple Book API.postman_collection.json`.
3. Update or verify the collection environment variables if needed.
4. Run individual requests or use a Postman Collection Runner.

## Notes

- `Submit an order`, `Get all orders`, `Update an order`, and `Delete an order` require bearer token authentication.
- `API Authentication` creates an API client and returns a token that can be used for order requests.
- `Single Book` uses a path variable `:ID` with a default value of `1`.
- `Update an order` and `Delete an order` use a path variable `:orderId` with sample values.
