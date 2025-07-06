# Smart Campus Complaint Management System

## Project Overview
The Smart Campus Complaint Management System is a MERN stack application designed to facilitate the management of complaints within a campus environment. This project focuses on Phase 1, which includes Authentication and User Management.

## Project Structure
The project is organized into two main directories: `client` for the React frontend and `server` for the Express backend.

```
smart-campus-complaint-system
├── client
│   ├── public
│   │   └── index.html
│   ├── src
│   │   ├── components
│   │   │   ├── Auth
│   │   │   │   ├── Login.jsx
│   │   │   │   └── Register.jsx
│   │   │   └── Navbar.jsx
│   │   ├── pages
│   │   │   ├── Home.jsx
│   │   │   └── Profile.jsx
│   │   ├── App.jsx
│   │   ├── index.jsx
│   │   └── api
│   │       └── auth.js
│   ├── package.json
│   └── README.md
├── server
│   ├── models
│   │   └── User.js
│   ├── routes
│   │   └── auth.js
│   ├── controllers
│   │   └── authController.js
│   ├── middleware
│   │   └── authMiddleware.js
│   ├── config
│   │   └── db.js
│   ├── app.js
│   ├── package.json
│   └── README.md
└── README.md
```

## Getting Started

### Prerequisites
- Install Node.js and npm if you haven't already.
- Set up MongoDB (either locally or via MongoDB Atlas).

### Setup Instructions
1. Create the project directory and navigate into it:
   ```
   mkdir smart-campus-complaint-system
   cd smart-campus-complaint-system
   ```

2. Create the React client:
   ```
   npx create-react-app client
   ```

3. Navigate to the server directory and initialize it:
   ```
   mkdir server
   cd server
   npm init -y
   ```

4. Install the necessary server dependencies:
   ```
   npm install express mongoose dotenv cors bcryptjs jsonwebtoken multer socket.io
   ```

5. Navigate to the client directory and install the necessary client dependencies:
   ```
   cd ../client
   npm install axios react-router-dom
   ```

### Running the Project
1. To run the server, navigate to the server directory and run:
   ```
   cd server
   node app.js
   ```

2. To run the client, navigate to the client directory and run:
   ```
   cd ../client
   npm start
   ```

This will start both the server and the client, allowing you to begin development on Phase 1: Authentication & User Management. 

## Features
- User registration and login functionality.
- Role-based access control for different user types (student, staff, admin).
- Basic navigation setup with a Navbar component.

## Future Enhancements
- Implement complaint submission and management features.
- Add user profile management capabilities.
- Enhance UI/UX for better user experience.