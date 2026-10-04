# SSR Styles – API

The backend for **SSR Styles**, a full-stack fashion e-commerce project. It serves the product catalogue, handles product image uploads, user signup and login, and keeps each user's cart in MongoDB.

Part of a three-repo project:

| Repo | Role |
|---|---|
| [SSR_Frontend](https://github.com/sunnykumar-devhub/SSR_Frontend) | Storefront for shoppers (React) |
| [SSRAdmin](https://github.com/sunnykumar-devhub/SSRAdmin) | Admin panel to add and list products |
| **SSRStyles** (this repo) | REST API (Node.js, Express, MongoDB) |

## API

| Method | Endpoint | Purpose |
|---|---|---|
| `POST` | `/upload` | Upload a product image (Multer) |
| `GET` | `/products` | List all products |
| `POST` | `/addproduct` | Add a product |
| `POST` | `/removeproduct` | Remove a product |
| `GET` | `/newcollection` | Latest products |
| `GET` | `/popularinwomen` | Popular products in the women category |
| `POST` | `/signup` | Create an account, returns a JWT |
| `POST` | `/login` | Log in, returns a JWT |
| `POST` | `/addtocart` | Add an item to the user's cart |
| `POST` | `/removefromcart` | Remove an item from the cart |
| `POST` | `/getcart` | Get the user's cart |

## Tech stack

Node.js · Express · MongoDB (Mongoose) · JSON Web Tokens · Multer · CORS · dotenv

## Getting started

```bash
npm install
node index.js
```

The server runs on `PORT` (default `5000`). Create a `.env` file with your MongoDB connection string and secrets before starting.

## Author

**Sunny Kumar**, Frontend Engineer · [Portfolio](https://sunnykdev.vercel.app) · [LinkedIn](https://www.linkedin.com/in/sunnykumar-devhub)
