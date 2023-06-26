# MERN E-commerce App

This is a MERN (MongoDB, Express.js, React.js, Node.js) e-commerce application that allows users to browse, purchase, and manage products. It features user authentication and role-based access control (RBAC), distinguishing between regular users and administrators.

## Backend

The backend of this application is implemented using Node.js and Express.js. It follows the MVC (Model-View-Controller) architectural pattern and includes the following components:

### Models

- User Model: Represents a user with properties such as name, email, password, and role. It is used for user authentication and authorization.
- Product Model: Represents a product with properties such as name, description, price, and image URL. It allows CRUD operations (Create, Read, Update, Delete) for managing products.
- Email Customer Model: Represents a customer's email details, which can be used for sending emails related to orders or promotions.

### API Routes

- User Routes: Handles user-related operations such as registration, login, and logout.
- Product Routes: Handles CRUD operations for managing products.
- Email Customer Routes: Handles email-related operations.

The backend also includes authentication middleware to ensure that only authenticated users can access certain routes. Additionally, it implements role-based access control, allowing different access levels for regular users and administrators.

## Frontend

The frontend of this application is built using React.js and is located in the `e-commerce` folder. It includes the following components:

### Pages

- Home Page: Displays featured products and other relevant information.
- Collection/Category Page: Shows a collection of products based on a specific category or collection.
- Single Product Detail Page: Displays detailed information about a specific product when clicked from the collection page.
- Register/Login/Logout: Provides functionality for user authentication and registration.

### Components

- Header: Navigational component that allows users to access different pages of the application.
- Admin Route: A protected route that can only be accessed by users with administrator roles. Provides access to additional functionality, such as managing products.

## Usage

To use this application, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/mern-ecommerce-app.git`
2. Install dependencies: `npm install`
3. Configure the backend:
   - Set up a MongoDB database and update the connection details in the `.env` file.
   - Configure any other necessary environment variables.
4. Start the backend server: `npm run server`
5. Configure the frontend:
   - Update the API endpoint in the frontend code to point to your backend server.
   - Configure any other necessary environment variables.
6. Start the frontend development server: `npm run start`
7. Access the application in your browser at `http://localhost:3000`.

Please note that you need to have Node.js and npm (Node Package Manager) installed on your system for the above steps to work.

## License

This project is licensed under the [MIT License](LICENSE).