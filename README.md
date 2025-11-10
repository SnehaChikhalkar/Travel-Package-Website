# Travel Package Website

## Overview
The Travel Package Website is a full-stack application that allows users to browse, book, and manage travel packages. The application consists of a backend built with Node.js and Express, and a frontend developed using React.

## Features
- User authentication (signup and login)
- Browse and search for travel packages
- View details of individual travel packages
- Book travel packages
- Protected routes for authenticated users

## Technologies Used
- **Backend**: Node.js, Express, MongoDB, Mongoose, JWT
- **Frontend**: React, Vite, Axios

## Folder Structure
```
travel-package-website/
├── backend/                # Backend server files
│   ├── package.json        # Backend dependencies and scripts
│   ├── server.js           # Entry point for the backend application
│   ├── .env                # Environment variables
│   ├── config/             # Configuration files
│   │   └── db.js           # MongoDB connection
│   ├── models/             # Mongoose schemas
│   │   ├── User.js         # User schema
│   │   ├── Package.js      # Travel package schema
│   │   └── Booking.js      # Booking schema
│   ├── routes/             # API routes
│   │   ├── authRoutes.js   # Authentication routes
│   │   ├── packageRoutes.js # Package CRUD routes
│   │   └── bookingRoutes.js # Booking routes
│   ├── controllers/        # Controller logic
│   │   ├── authController.js # Auth logic
│   │   ├── packageController.js # Package logic
│   │   └── bookingController.js # Booking logic
│   ├── middleware/         # Middleware functions
│   │   └── authMiddleware.js # JWT verification
│   └── utils/              # Utility functions
│       └── generateToken.js # JWT helper
│
├── frontend/               # Frontend application files
│   ├── package.json        # Frontend dependencies and scripts
│   ├── vite.config.js      # Vite configuration
│   ├── src/                # Source files for React app
│   │   ├── main.jsx        # Entry point for the React application
│   │   ├── App.jsx         # Main App component
│   │   ├── components/     # Reusable components
│   │   │   ├── Navbar.jsx
│   │   │   ├── PackageCard.jsx
│   │   │   ├── BookingForm.jsx
│   │   │   └── ProtectedRoute.jsx
│   │   ├── pages/          # Page components
│   │   │   ├── Home.jsx
│   │   │   ├── Packages.jsx
│   │   │   ├── PackageDetails.jsx
│   │   │   ├── Booking.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Register.jsx
│   │   ├── services/       # API service files
│   │   │   └── api.js
│   │   └── context/        # Context API files
│   │       └── AuthContext.jsx
│   └── public/             # Public files
│       └── index.html      # Main HTML file
│
├── README.md               # Project documentation
└── .gitignore              # Git ignore file
```

## Setup Instructions
1. Clone the repository:
   ```
   git clone <repository-url>
   ```
2. Navigate to the backend directory and install dependencies:
   ```
   cd backend
   npm install
   ```
3. Create a `.env` file in the backend directory and add your environment variables.
4. Start the backend server:
   ```
   npm start
   ```
5. Navigate to the frontend directory and install dependencies:
   ```
   cd ../frontend
   npm install
   ```
6. Start the frontend application:
   ```
   npm run dev
   ```

## License
This project is licensed under the MIT License.