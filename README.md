
# Car Rentals Project

A car rental management system built with the MERN (MongoDB, Express, React, Node.js) stack. This application allows users to browse, book, and manage car rentals. Admin users can manage car listings, bookings, and user data.

## Features

- **User Management**: Sign up, log in, and profile management.
- **Car Listings**: Browse and search available cars.
- **Booking System**: Rent a car, manage bookings.
- **Admin Dashboard**: Manage car listings, view bookings, and handle user data.

---

## Project Structure

- **Frontend**: Built with React and styled using CSS frameworks. Provides user views for browsing cars, managing rentals, and handling payments.
- **Backend**: Built with Node.js, Express, and MongoDB. Implements RESTful API endpoints for user and booking management.

---

## Prerequisites

- **Node.js** (v14+)
- **MongoDB** (Local or hosted like MongoDB Atlas)
- **React** (Frontend)
- **Express** (Backend)

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/JulakantiManith/car-rentals.git
cd car-rentals
```

### 2. Install Dependencies

#### Frontend
Navigate to the `client` directory and install dependencies:

```bash
cd client
npm install
```

#### Backend
Navigate to the `server` directory and install dependencies:

```bash
cd server
npm install
```

### 3. Set Up Environment Variables

#### Backend
Create a `.env` file in the `server` directory with the following configuration:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/car_rentals # or your MongoDB Atlas URL
JWT_SECRET=your_jwt_secret
```

#### Frontend
In the `client` directory, create a `.env` file:

```env
REACT_APP_API_URL=http://localhost:5000
```

---

## Running the Project

### Start Frontend and Backend Together

In the backend i.e client, use the following command to start both the frontend and backend at once:

```bash
npm run dev
```

- This command assumes a script is set up in the root `package.json` file to run both `client` and `server` concurrently.

### 3. Access the Application

- Frontend: Open [http://localhost:3000](http://localhost:3000) in your browser.
- Backend: API will be running on [http://localhost:5000](http://localhost:5000).

---

## API Endpoints (Backend)

Here’s a brief overview of the key API endpoints:

- **Auth Routes** (`/api/auth`)
  - `POST /login` - Log in a user
  - `POST /register` - Register a new user
- **Car Routes** (`/api/cars`)
  - `GET /` - Get all cars
  - `POST /` - Add a new car (Admin only)
  - `PUT /:id` - Update car details (Admin only)
  - `DELETE /:id` - Delete a car (Admin only)
- **Booking Routes** (`/api/bookings`)
  - `POST /` - Create a new booking
  - `GET /user/:id` - Get bookings by user
  - `DELETE /:id` - Cancel a booking

---

## Usage

1. **User Actions**: Register or log in, search for available cars, and make bookings.
2. **Admin Actions**: Add, update, or delete car listings and manage bookings.

---

## Built With

- **MongoDB** - Database for storing user, car, and booking information
- **Express** - Node.js framework for building RESTful APIs
- **React** - Frontend framework for building user interfaces
- **Node.js** - JavaScript runtime for server-side development

---


## License

This project is open-source and available under the MIT License.
