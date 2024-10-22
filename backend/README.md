# Expenses Tracker API

A scalable RESTful API built with Node.js and Express for managing expenses, featuring user authentication, role-based access control, and advanced filtering capabilities.

## Features

- CRUD operations for expenses
- Advanced filtering (by category, date range, payment method)
- Sorting and pagination for large datasets
- User authentication and authorization using JWT
- Role-based access control (Admin vs. Regular User)
- Secure password hashing with bcrypt
- Bulk upload of expenses via CSV
- Comprehensive error handling and logging
- In-memory caching for optimized performance

## Technologies Used

- Node.js
- Express
- MongoDB
- Mongoose
- JSON Web Token (JWT)
- Bcrypt.js
- dotenv
- multer
- Redis

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Sujanbutani/Expenses-Tracker-App-p-8.git

2. Install dependencies:

    ```bash
    npm install

3. .env file

     ```
    MONGO_URI=your_mongo_db_connection_string
    PORT=5000
    JWT_SECRET=your_jwt_secret_key

    ```

4. Start the development server:

   ```bash
   npm start
   The server should now be running at http://localhost:5000
   ```

## API Endpoints

### User Authentication
1. SingUp User (Post) :- localhost:5000/api/auth/signup
2. Login User (Post) :- localhost:5000/api/auth/login

### Event Management
1. Expenses Api (Post) :- localhost:5000/api/expenses
    - Requires JWT token in the Authorization header.
2. Expenses Api (Post - bulk) :- localhost:5000/api/expenses/bulk
3. Expenses Api (Get - All) :-  localhost:5000/api/expenses
4. Expenses Api (PATCH - Update) :- localhost:5000/api/expenses/<expenses_Id>
5. Expenses Api (Delete) :- localhost:5000/api/expenses/<expenses_Id>

## Environment Variables
- PORT: The port for the server to listen on.
- MONGODB_URI: Your MongoDB connection string.
- JWT_SECRET: Secret key for signing JWT tokens.