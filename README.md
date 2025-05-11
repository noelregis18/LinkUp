# LinkUp - Social Media Platform

## Overview
LinkUp is a modern social media platform built with the MERN stack (MongoDB, Express.js, React, Node.js). It allows users to connect with friends, share posts, and interact with content in a user-friendly interface.

## Features

### User Authentication
- Secure registration and login system
- Email verification
- Password reset functionality
- JWT-based authentication

### Profile Management
- Customizable user profiles
- Profile picture upload via Cloudinary
- Edit personal information (name, profession, location)
- Profile view tracking

### Social Interactions
- Send and accept friend requests
- View suggested friends
- Create and share posts
- Like and comment on posts
- View user timelines

### User Interface
- Responsive design for all devices
- Modern UI with Tailwind CSS
- Dark/light theme support

## Project Structure

```
LinkUp/
├── client/               # Frontend React application
│   ├── public/           # Static files
│   └── src/              # React source code
│       ├── components/   # Reusable UI components
│       ├── pages/        # Application pages
│       ├── redux/        # State management
│       └── utils/        # Utility functions
└── server/               # Backend Node.js/Express application
    ├── controllers/      # Request handlers
    ├── middlewares/      # Express middlewares
    ├── models/           # MongoDB schemas
    ├── routes/           # API routes
    └── utils/            # Utility functions
```

## Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- npm or yarn

### Setup Instructions

1. Clone the repository

2. Install server dependencies
   ```bash
   cd server
   npm install
   ```

3. Configure environment variables
   Create a `.env` file in the server directory with the following variables:
   ```
   PORT=8008
   MONGODB_URL=your_mongodb_connection_string
   JWT_SECRET_KEY=your_jwt_secret
   EMAIL_USER=your_email_for_sending_verification
   EMAIL_PASS=your_email_password
   ```

4. Install client dependencies
   ```bash
   cd ../client
   npm install
   ```

5. Configure client environment variables
   Create a `.env` file in the client directory with:
   ```
   VITE_APP_API_URL=http://localhost:8008
   VITE_CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   VITE_CLOUDINARY_UPLOAD_PRESET=your_cloudinary_upload_preset
   ```

## Running the Application

1. Start the server
   ```bash
   cd server
   npm run dev
   ```

2. Start the client
   ```bash
   cd client
   npm run dev
   ```

3. Open your browser and navigate to `http://localhost:5173`

## Technologies Used

### Frontend
- React.js
- Redux Toolkit for state management
- React Router for navigation
- Tailwind CSS for styling
- Axios for API requests
- React Hook Form for form handling

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Bcrypt for password hashing
- Nodemailer for email services

### Cloud Services
- Cloudinary for image storage

## License
ISC