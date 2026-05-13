# E‑commerce Back End

Back end for an e‑commerce site built with Express.js, Sequelize, and MySQL.



## Technologies

- Node.js + Express.js
- Sequelize ORM
- MySQL2
- dotenv

## Installation

1. Clone the repo  
   `git clone https://github.com/your-username/your-repo.git`

2. Install dependencies  
   `npm install`

3. Create a `.env` file in the root:  

DB_NAME=ecommerce_db
DB_USER=root
DB_PW=your_mysql_password


4. Create the database (in MySQL shell or Workbench):  
`CREATE DATABASE ecommerce_db;`

5. Seed the database  
`npm run seed`

6. Start the server  
`npm start`

## API Routes

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | `/api/categories` | Get all categories (includes products) |
| GET    | `/api/categories/:id` | Get one category |
| POST   | `/api/categories` | Create a category |
| PUT    | `/api/categories/:id` | Update a category |
| DELETE | `/api/categories/:id` | Delete a category |
| GET    | `/api/products` | Get all products (includes category and tags) |
| GET    | `/api/products/:id` | Get one product |
| POST   | `/api/products` | Create a product (with `tagIds` array) |
| PUT    | `/api/products/:id` | Update a product |
| DELETE | `/api/products/:id` | Delete a product |
| GET    | `/api/tags` | Get all tags (includes products) |
| GET    | `/api/tags/:id` | Get one tag |
| POST   | `/api/tags` | Create a tag |
| PUT    | `/api/tags/:id` | Update a tag |
| DELETE | `/api/tags/:id` | Delete a tag |

## Insomnia Collection

Import `insomnia-collection.yaml` into [Insomnia Core](https://insomnia.rest) to test all routes instantly.

1. Open Insomnia → **Import/Export** → **Import Data** → **From File**
2. Select `insomnia-collection.yaml`

## License

MIT

## Author
Jeevan Thapa
