# Running Bun With MongoDB

This is a sample project demonstrating how to use Bun server with MongoDB to create a simple movie database API.

## Prerequisites

- [Bun](https://bun.sh) installed on your system
- A MongoDB database (you can use MongoDB Atlas for a free cloud-hosted option)

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/tooniez/bun-api-mongodb
   cd bun-api-mongodb
   ```

2. Install dependencies:
   ```bash
   bun install
   ```

3. Set up your environment variables:
   Copy `.env.example` file in the root directory and add your MongoDB connection string:
   ```
   cp .env.example .env
   MONGODB_URI=<your_mongodb_connection_string>
   ```

4. Run the application:
   ```bash
   bun run index.ts
   ```

## API Endpoints

- `GET /movies`: Fetch all movies
- `GET /movies/:id`: Fetch a specific movie by ID
- `POST /movies`: Add a new movie
- `PUT /movies/:id`: Update a movie
- `DELETE /movies/:id`: Delete a movie

## Project Structure

- `index.ts`: Main application file with route handlers
- `controllers/movies.ts`: Movie controller with CRUD operations
- `models/movies.ts`: Movie model definition
- `utils/db.ts`: Database connection utility

## Docker Support

If you prefer to use Docker, you can run the project using the `oven/bun` image:

## License

📝 Copyright © 2024 [tooniez](https://github.com/tooniez). <br />
This project is [MIT](https://github.com/tooniez/bun-api-mongodb`/blob/main/LICENSE) licensed.