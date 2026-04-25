# BloodConnect: Blood Bank Management System

BloodConnect is a comprehensive Blood Bank Management System built using the MERN (MongoDB, Express.js, React.js, Node.js) stack. It streamlines the process of managing blood donations, tracking inventory, and fulfilling blood requests from hospitals or individuals.

## 🌟 Features

- **Role-Based Access Control:** Separate dashboards and functionalities for:
  - **Admin:** Manage entire system, users, inventory, and requests.
  - **Donor:** Track donation history and view upcoming blood camps.
  - **Hospital:** Submit blood requests and track status.
  - **Organization:** Manage blood donation camps and bulk donations.
- **Real-Time Updates:** Built with Socket.io for instant notifications on blood requests and inventory changes.
- **Inventory Management:** Live tracking of blood groups (A+, B+, O+, O-, etc.) and their availability.
- **Secure Authentication:** JWT-based authentication and secure password hashing.
- **Responsive UI:** Clean, modern, and mobile-friendly interface built with React and Tailwind CSS.

## 🛠️ Tech Stack

**Frontend:**
- React.js (Vite)
- Tailwind CSS
- React Router DOM
- Framer Motion (Animations)
- Socket.io Client

**Backend:**
- Node.js & Express.js
- MongoDB & Mongoose
- Socket.io
- JSON Web Tokens (JWT) & bcrypt.js

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) installed on your machine
- [MongoDB](https://www.mongodb.com/) running locally or a MongoDB Atlas URI

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Kandikarthik/Blood-Bank-Management-System.git
   cd Blood-Bank-Management-System
   ```

2. **Backend Setup**
   ```bash
   cd server
   npm install
   ```
   Create a `.env` file in the `server` directory:
   ```env
   PORT=5001
   MONGODB_URI=mongodb://127.0.0.1:27017/bloodconnect
   NODE_ENV=development
   JWT_SECRET=your_jwt_secret_key_here
   ```
   Start the backend server:
   ```bash
   npm run dev
   ```

3. **Frontend Setup**
   Open a new terminal window:
   ```bash
   cd client
   npm install
   ```
   Create a `.env` file in the `client` directory:
   ```env
   VITE_API_BASE_URL=http://localhost:5001/api
   VITE_SOCKET_URL=http://localhost:5001
   ```
   Start the frontend client:
   ```bash
   npm run dev
   ```

4. **Access the Application**
   Open your browser and navigate to `http://localhost:5173`.

### 🔑 Default Admin Credentials
When you run the backend for the first time, it automatically creates an admin account:
- **Email:** `admin@bloodconnect.com`
- **Password:** `admin123`

## 🤝 Contributing
Contributions, issues, and feature requests are welcome!