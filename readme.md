# 🎯 Job Portal Application

<div align="center">

![React](https://img.shields.io/badge/React-18.2.0-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-14+-green.svg)
![MongoDB](https://img.shields.io/badge/MongoDB-8.4.1-brightgreen.svg)
![License](https://img.shields.io/badge/License-ISC-blue.svg)

A modern full-stack job portal application that connects job seekers with employers, featuring a beautiful UI and robust backend functionality.

[![Deploy](https://img.shields.io/badge/Deploy-Live-green)](https://your-deployment-url.com)
[![Stars](https://img.shields.io/github/stars/yourusername/jobportal-yt?style=social)](https://github.com/yourusername/jobportal-yt)

</div>

## ✨ Features

- 🔐 User Authentication (Job Seeker & Employer)
- 💼 Job Posting and Management
- 🔍 Job Search and Filtering
- 👤 Profile Management
- 📝 Application Tracking
- 🎨 Modern and Responsive UI
- 🌓 Dark/Light Mode Support

## 🛠️ Tech Stack

### Frontend
- ⚛️ React.js with Vite
- 🔄 Redux Toolkit for State Management
- 🛣️ React Router for Navigation
- 🎨 Tailwind CSS for Styling
- 🎯 Radix UI Components
- ✨ Framer Motion for Animations
- 🔌 Axios for API Calls

### Backend
- 🚀 Node.js
- ⚡ Express.js
- 📦 MongoDB with Mongoose
- 🔑 JWT Authentication
- ☁️ Cloudinary for Image Upload
- 📁 Multer for File Handling
- 🔒 Bcrypt for Password Hashing

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Ashish-Code-01/Job-portal
cd jobportal
```

2. Install Backend Dependencies:
```bash
cd backend
npm install
```

3. Install Frontend Dependencies:
```bash
cd ../frontend
npm install
```

4. Create a `.env` file in the backend directory with the following variables:
```env
PORT=5000
MONGO_URI=your_mongodb_uri
SECRET_KEY=your_jwt_secret
CLOUD_NAME=your_cloudinary_cloud_name
API_KEY=your_cloudinary_api_key
API_SECRET=your_cloudinary_api_secret
```

### Running the Application

1. Start the Backend Server:
```bash
cd backend
npm run dev
```

2. Start the Frontend Development Server:
```bash
cd frontend
npm run dev
```

The application will be available at:
- 🌐 Frontend: http://localhost:5173
- 🔧 Backend: http://localhost:5000

## 📁 Project Structure

```
jobportal-yt/
├── frontend/
│   ├── src/
│   │   ├── assets/         # Static assets
│   │   ├── components/     # Reusable UI components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── lib/           # Utility libraries
│   │   ├── redux/         # Redux store and slices
│   │   └── utils/         # Helper functions
│   ├── public/            # Public assets
│   └── package.json
└── backend/
    ├── controllers/       # Route controllers
    ├── models/           # MongoDB models
    │   ├── application.model.js
    │   ├── company.model.js
    │   ├── job.model.js
    │   └── user.model.js
    ├── routes/           # API routes
    ├── middlewares/      # Custom middlewares
    ├── utils/           # Helper functions
    └── package.json
```

## 🔌 API Documentation

### Base URL
```
http://localhost:8000/api/v1
```

### Authentication Endpoints

#### User Routes
- `POST /user/register` - Register a new user
- `POST /user/login` - Login user
- `GET /user/logout` - Logout user
- `POST /user/profile/update` - Update user profile (requires authentication)

#### Job Routes
- `POST /job/post` - Post a new job (requires authentication)
- `GET /job/get` - Get all jobs (requires authentication)
- `GET /job/getadminjobs` - Get jobs posted by admin (requires authentication)
- `GET /job/get/:id` - Get job by ID (requires authentication)

#### Application Routes
- `GET /application/apply/:id` - Apply for a job (requires authentication)
- `GET /application/get` - Get all applied jobs (requires authentication)
- `GET /application/:id/applicants` - Get applicants for a job (requires authentication)
- `POST /application/status/:id/update` - Update application status (requires authentication)

### Request/Response Format

#### Authentication
```json
// Register Request
{
  "name": "string",
  "email": "string",
  "password": "string",
  "role": "user" | "admin"
}

// Login Request
{
  "email": "string",
  "password": "string"
}
```

#### Job
```json
// Post Job Request
{
  "title": "string",
  "description": "string",
  "company": "string",
  "location": "string",
  "salary": "string",
  "type": "string"
}
```

#### Application
```json
// Update Status Request
{
  "status": "pending" | "accepted" | "rejected"
}
```

### Authentication
- All protected routes require a valid JWT token
- Token should be included in the Authorization header
- Format: `Authorization: Bearer <token>`

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. 🍴 Fork the repository
2. 🌿 Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. 💾 Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. 📤 Push to the branch (`git push origin feature/AmazingFeature`)
5. 🔄 Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

---

<div align="center">
Made with ❤️ by [Ashis Vishwakarma]
</div> 
#   J o b - p o r t a l  
 