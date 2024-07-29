# Trello-Style Task Management Application

This is a full-stack Task Management Application built with **Next.js** for the frontend and **Node.js** with **Express** and **MongoDB** for the backend. The application allows users to register, log in, and manage tasks with features such as creating, updating, deleting, and retrieving tasks.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Backend Setup](#backend-setup)
  - [Frontend Setup](#frontend-setup)
- [API Endpoints](#api-endpoints)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- User registration and authentication
- Create, read, update, and delete tasks
- Task categorization with status and priority
- Responsive design for mobile and desktop

## Technologies Used

- **Frontend**: 
  - Next.js
  - React
  - TypeScript
  - Axios
  - Tailwind CSS
  - React Hot Toast for toasts

- **Backend**: 
  - Node.js
  - Express
  - MongoDB with Mongoose
  - JSON Web Token (JWT) for authentication
  - Bcrypt for hashing passwords
  - nodemon for local development

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB (local or cloud instance)
- npm or yarn

Clone the repository
```bash
   git clone https://github.com/Abhi6722/crework.git
   cd crework
   ```

### Backend Setup

1. **Cd into the folder**:

   ```bash
   cd backend
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Create a `.env` file** in the `backend` directory and add the following environment variables:

   ```plaintext
   PORT=8080
   MONGODB_URI=mongodb://localhost:27017/task_management
   JWT_SECRET=your_jwt_secret
   ```

   Replace `your_jwt_secret` with a secure secret key.

4. **Start the backend server**:

   ```bash
   npm run dev
   ```

   The backend server will run on `http://localhost:8080`.


### Frontend Setup

1. **Navigate to the frontend directory**:

   ```bash
   cd ../frontend
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Create a `.env.local` file** in the `frontend` directory and add the following environment variable:

   ```plaintext
   NEXT_PUBLIC_BACKEND_URL=http://localhost:8080
   ```

4. **Start the frontend server**:

   ```bash
   npm run dev
   ```

   The frontend application will run on `http://localhost:3000`.


## API Endpoints
You can find the postman collection for all the endpoints in file postman.json inside the backend folder. You can import in the postman, create an environment and just create a empty variable with name token. After activating the token you can use the APIs. You need to first register/login to get the jwt access token that will be used to later handle other requests.

## Usage

1. Register a new user using the registration endpoint.
2. Log in to receive a JWT token.
3. Use the token to access task management endpoints.
4. Create, update, delete, and retrieve tasks as needed.
