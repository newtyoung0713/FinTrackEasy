# FinTrackEasy

FinTrackEasy is a user-friendly personal finance tracking application that helps users manage their daily income and expenses.

# Member
| Name | ID |
|:---:|:---:|
| Aaron Liu ||
| Carrie Leung ||
| Wing Ho Chau ||
| Sheng-Lin Yang ||

## Project Structure

```
FinTrackEasy/  
├── fte-react/          # Frontend React Application
│   ├── public/         # Static Resources
│   ├── src/           
│   │   ├── components/ # UI Components
│   │   ├── pages/     # Feature Pages
│   │   ├── services/  # API Request Encapsulation
│   │   └── App.js     # Main Application Component
│   └── package.json    # Frontend Dependencies
│  
├── express/            # Backend Express Service
│   ├── config/        # MongoDB Connection and Configuration
│   ├── models/        # Mongoose Schema (User, Account, Expense, Income...)
│   ├── routes/        # API Routes
│   ├── controllers/   # Business Logic and Data Operations
│   ├── middlewares/   # Middleware (Validation/Error Handling)
│   ├── utils/         # Utility Modules
│   ├── app.js         # Express Application Configuration
│   └── server.js      # Server Entry Point
│  
├── .env               # Environment Variables
└── README.md          # Project Documentation
```

## Technology Stack

### Frontend
- React
- React Router
- Axios
- Shadcn UI/Tailwind CSS

### Backend
- Node.js
- Express
- MongoDB
- Mongoose

## Installation Guide

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- pnpm

### Installation Steps

1. Clone the project
```bash
git clone [repository-url]
cd FinTrackEasy
```

2. Install backend dependencies
```bash
cd express
pnpm install
```

3. Install frontend dependencies
```bash
cd ../fte-react
pnpm install
```

4. Configure environment variables
Create a `.env` file in the project root directory and add the necessary environment variables:
```
MONGODB_URI=your_mongodb_connection_string
PORT=3000
```

## Running the Project

### Start Backend Service
```bash
cd express
pnpm start
```

### Start Frontend Development Server
```bash
cd fte-react
pnpm dev
```

## API Documentation

### User Related
- POST /api/auth/register - User Registration
- POST /api/auth/login - User Login
- GET /api/auth/profile - Get User Profile

### Financial Records
- GET /api/transactions - Get Transaction Records
- POST /api/transactions - Create New Transaction
- PUT /api/transactions/:id - Update Transaction
- DELETE /api/transactions/:id - Delete Transaction

## Contributing Guidelines

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details