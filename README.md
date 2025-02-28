# Backend Fundamentals Project

This is a backend project built with Node.js and the Fastify. It uses Knex for database interactions and Zod for schema validation.

## Project Deployment

The project is deployed at: [https://zero2-api-rest-nodejs-z216.onrender.com/](https://zero2-api-rest-nodejs-z216.onrender.com/)

## API Routes

### POST /transactions

Create a new transaction.

#### Request Body

```json
{
  "title": "dev service",
  "amount": 200,
  "type": "debit"
}
```

Create a new transaction.

### GET /transactions/summary

Retrieve a summary of all transactions.

### GET /transactions/:id

Retrieve a specific transaction by its ID.

Example: `/transactions/dab91a11-0ffc-4864-8f1a-32a46dd6bed5`

### GET /transactions

Retrieve all transactions.

## Technologies Used

- Node.js
- Fastify
- Knex
- Zod

## Getting Started

To get started with the project, clone the repository and install the dependencies:

```bash
git clone https://github.com/Cassiano26/02-api-rest-nodeJS.git
cd 02-api-rest-nodeJS
npm install
npm run knex -- migrate:latest
```


## Running the Project

To run the project locally, use the following command:

```bash
npm run dev
```

## Environment Variables

The project requires the following environment variables, which can be found in the `.env.example` file:

```plaintext
DATABASE_URL="./db/app.db"
DATABASE_CLIENT=sqlite
PORT=3333
```

By default, the application will run on `http://localhost:3333` during development.

## License

This project is licensed under the MIT License.