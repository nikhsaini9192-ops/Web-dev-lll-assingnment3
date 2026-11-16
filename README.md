# Inventory and Data Management System
Run: `npm install` then `npm start` (needs MongoDB running locally).

| Method | Endpoint | Purpose |
|---|---|---|
| POST | /api/products | Create product |
| GET | /api/products | List (filter, sort, paginate) |
| GET | /api/products/:id | Single product |
| PUT | /api/products/:id | Update product |
| PATCH | /api/products/:id/stock | Body `{"change": 10}` restock / `{"change": -3}` sale |
| DELETE | /api/products/:id | Delete |
| GET | /api/products/low-stock | quantity <= reorderLevel |
| GET | /api/products/summary | Category-wise aggregation |

Query examples: `?category=Furniture&minPrice=100&sort=-price&page=1&limit=10`
