# Friends-Bazaar
Website for my shop
# MERN Stack E-Commerce Application

Welcome to the MERN Stack E-Commerce Application! This project demonstrates a full-stack web application built using the MERN stack (MongoDB, Express.js, React.js, and Node.js). It serves as a comprehensive guide for beginners and intermediate developers to understand and implement a responsive and dynamic e-commerce platform.

---

## Features

- **User Authentication**: Secure user registration and login using JWT.
- **Product Management**: CRUD operations for product listings.
- **Shopping Cart**: Add, remove, and update cart items.
- **Order Management**: Place and manage orders.
- **Payment Integration**: Integrated payment gateway for seamless transactions.
- **Admin Dashboard**: Manage products, orders, and users.
- **Responsive Design**: Fully responsive interface for all devices.
- **RESTful API**: Modular and scalable backend API using Express.js.
- **Database**: Efficient data handling with MongoDB.

---

## Technologies Used

- **Frontend**:
  - React.js (Hooks, Context API)
  - React Router for routing
  - Tailwind CSS/Bootstrap for styling

- **Backend**:
  - Node.js
  - Express.js
  - JSON Web Tokens (JWT) for authentication
  - Bcrypt for password hashing

- **Database**:
  - MongoDB (Mongoose as ORM)

- **Tools & Libraries**:
  - Axios for API calls
  - Redux (optional for state management)
  - Stripe/PayPal API for payments (configurable)

---

## Installation and Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/PrinceKumar182/Friends-Bazaar
   cd mern-ecommerce-app
   ```

2. **Install dependencies**:
   - Backend:
     ```bash
     cd backend
     npm install
     ```
   - Frontend:
     ```bash
     cd frontend
     npm install
     ```

3. **Environment Variables**:
   Create a `.env` file in the root of the `backend` directory and add the following:
   ```env
   MONGO_URI=<your-mongodb-connection-string>
   JWT_SECRET=<your-jwt-secret>
   PORT=5000
   STRIPE_SECRET_KEY=<your-stripe-secret-key>
   ```

4. **Run the Application**:
   - Start the backend server:
     ```bash
     cd backend
     npm run dev
     ```
   - Start the frontend development server:
     ```bash
     cd frontend
     npm start
     ```

5. **Access the Application**:
   Open your browser and navigate to `http://localhost:3000`.

---

## Folder Structure

```
mern-ecommerce-app/
├── backend/
│   ├── config/           # MongoDB and other configurations
│   ├── controllers/      # API controllers
│   ├── models/           # Mongoose models
│   ├── routes/           # Express routes
│   └── server.js         # Main server file
│
├── frontend/
│   ├── public/           # Public assets
│   ├── src/
│   │   ├── components/   # Reusable components
│   │   ├── pages/        # Page components
│   │   ├── context/      # Context API files
│   │   └── App.js        # Root component
│   └── package.json
│
└── README.md             # Project documentation
```

---

## Future Enhancements

- Implement user reviews and ratings for products.
- Add product filtering and sorting options.
- Introduce real-time notifications using WebSockets.
- Implement a wish list feature.
- Deploy the application using services like AWS, Heroku, or Vercel.

---

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or new features.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Author

Developed by **Prince Kumar** and the MERN Stack community.

Happy Coding! 🚀
