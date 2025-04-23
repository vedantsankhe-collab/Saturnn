# SATURN - Modern Expense Tracker Application



## 🌟 Overview

saturn is a comprehensive expense tracking solution designed to help users manage their finances with ease. This full-stack web application combines beautiful UI with powerful functionality to provide an intuitive financial management experience.

Whether you're planning a budget for the month, tracking daily expenses, or analyzing your spending habits, SpendSmart has got you covered.



## ✨ Key Features

### 📊 Dashboard & Stats
- **Financial Overview**: Get a bird's-eye view of your finances with total budget amounts, spending, and budget count
- **Interactive Charts**: Visualize your financial data with dynamic bar charts showing your latest five budgets
- **Recent Activity**: Quick access to your latest transactions and budget updates

### 💰 Budget Management
- **Create Custom Budgets**: Set up budgets with custom names, amounts, and even personalize with emojis
- **Detailed Budget View**: Dive into each budget to see all transactions associated with it
- **Budget Modification**: Easily update or delete budgets as your financial plans change

### 💸 Expense Tracking
- **Comprehensive Expense Logs**: View all your expenses in one organized table
- **Categorized Expenses**: Assign expenses to specific budgets for better organization
- **Edit & Delete**: Maintain accuracy by editing or removing expense entries

### 🔐 User Authentication
- **Secure Login**: Traditional email/password authentication
- **Google Integration**: Quick sign-in with Google account
- **Persistent Sessions**: JWT token storage in cookies for seamless user experience

## 🛠️ Technology Stack

### Frontend
- **React**: Powers the interactive user interface with component-based architecture
- **Redux Toolkit**: Manages global state across the application for a consistent user experience
- **TailwindCSS**: Enables rapid UI development with utility-first approach
- **Chart.js & React-Chartjs-2**: Creates beautiful and responsive data visualizations
- **Axios**: Handles HTTP requests to the backend APIs
- **Firebase Authentication**: Provides secure Google sign-in functionality
- **Vite**: Delivers fast development experience and optimized builds

### Backend
- **Node.js**: JavaScript runtime for server-side execution
- **Express**: Fast, unopinionated web framework for building RESTful APIs
- **MongoDB**: NoSQL database for flexible data storage
- **Mongoose**: Object modeling tool for MongoDB data
- **JWT (JSON Web Tokens)**: Secures API endpoints and manages user sessions
- **bcryptjs**: Handles password hashing for secure user authentication
- **Cookie-parser**: Parses cookies for JWT token storage and retrieval

## 📡 API Reference

### Authentication Endpoints
- `POST /api/auth/signup`: Register new user
- `POST /api/auth/signin`: Authenticate existing user
- `POST /api/auth/google-oauth`: Authenticate with Google
- `GET /api/auth/get/user`: Retrieve current user profile
- `DELETE /api/auth/signout`: Log out user

### Budget Endpoints
- `GET /api/budget/get`: Retrieve all budgets for current user
- `GET /api/budget/get/:id`: Get specific budget details
- `POST /api/budget/add`: Create new budget
- `PUT /api/budget/update/:id`: Update existing budget
- `DELETE /api/budget/delete/:id`: Remove budget

### Expense Endpoints
- `GET /api/expense/get`: Fetch all expenses
- `GET /api/expense/get/:budgetId`: Get expenses for specific budget
- `POST /api/expense/add`: Create new expense
- `PUT /api/expense/update/:id`: Update existing expense
- `DELETE /api/expense/delete/:id`: Remove expense

### Stats Endpoints
- `GET /api/stats/overview`: Retrieve financial statistics and overview

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or later)
- MongoDB database (local or Atlas)
- Firebase project (for Google Authentication)

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/vedantsankhe-collab/Saturnn.git
   cd Saturnn
   ```

2. **Install dependencies**
   ```bash
   # Install server dependencies
   cd server
   npm install

   # Install client dependencies
   cd ../client
   npm install
   ```

3. **Environment setup**

   Server (.env):
   ```
   MONGO_URI=mongodb+srv://<username>:<password>@<cluster>.mongodb.net/<database>
   SALT=16
   JWT_SECRET=your_jwt_secret_key
   CLIENT_URL=http://localhost:5173
   ```

   Client (.env):
   ```
   VITE_FIREBASE_API_KEY=your_firebase_api_key
   VITE_API_URL=http://localhost:3000
   ```

4. **Running the application**
   ```bash
   # Start the server
   cd server
   npm start
   
   # Start the client in a new terminal
   cd client
   npm run dev
   ```

5. **Access the application**
   Open your browser and navigate to http://localhost:5173

## 📝 License

This project is licensed under the MIT License.

## 🙏 Acknowledgements

- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [MongoDB Documentation](https://docs.mongodb.com/)
- [Express Documentation](https://expressjs.com/)
- [TailwindCSS Documentation](https://tailwindcss.com/docs)
- [Redux Toolkit Documentation](https://redux-toolkit.js.org/)
