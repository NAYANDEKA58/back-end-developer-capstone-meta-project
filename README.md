# Little Lemon Restaurant API

Welcome to the Little Lemon Restaurant API. This project provides endpoints for user authentication, menu item management, and table bookings.

## 1. User Registration & Authentication (Djoser)

| HTTP Method | Endpoint | Description |
| --- | --- | --- |
| **POST** | `[http://127.0.0.1:8000/auth/users/](http://127.0.0.1:8000/auth/users/)` | Register a new user account. |
| **POST** | `[http://127.0.0.1:8000/restaurant/api-token-auth/](http://127.0.0.1:8000/restaurant/api-token-auth/)` | Log in with credentials to obtain an authentication token. |

---

## 2. Menu Items API

These endpoints handle the retrieval and modification of Little Lemon's menu items.

| HTTP Method | Endpoint | Description |
| --- | --- | --- |
| **GET** | `[http://127.0.0.1:8000/restaurant/menu/](http://127.0.0.1:8000/restaurant/menu/)` | List all menu items. |
| **POST** | `[http://127.0.0.1:8000/restaurant/menu/](http://127.0.0.1:8000/restaurant/menu/)` | Add a new menu item. |
| **GET** | `[http://127.0.0.1:8000/restaurant/menu/](http://127.0.0.1:8000/restaurant/menu/)<id>` | Retrieve a specific menu item by its ID. |
| **PUT** | `[http://127.0.0.1:8000/restaurant/menu/](http://127.0.0.1:8000/restaurant/menu/)<id>` | Update an entire menu item. |
| **DELETE** | `[http://127.0.0.1:8000/restaurant/menu/](http://127.0.0.1:8000/restaurant/menu/)<id>` | Remove a menu item. |

---

## 3. Booking API

> 🔒 **Authentication Required:** You must provide a valid authorization token in the HTTP header to access the booking endpoints.

| HTTP Method | Endpoint | Description |
| --- | --- | --- |
| **GET** | `[http://127.0.0.1:8000/restaurant/booking/tables/](http://127.0.0.1:8000/restaurant/booking/tables/)` | List all table bookings. |
| **POST** | `[http://127.0.0.1:8000/restaurant/booking/tables/](http://127.0.0.1:8000/restaurant/booking/tables/)` | Create a new table booking. |

### How to Authenticate in API Clients (Insomnia / Postman)

When testing the Booking endpoints, add the following key-value pair under the **Headers** tab:

* **Key:** `Authorization`
* **Value:** `Token <your_generated_token_string>`

*(Make sure there is a space between the word `Token` and your actual token string!)*
