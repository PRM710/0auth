# OAUTH

This project contains a full-stack application with a frontend and backend. Follow the instructions below to set up and run the project locally.

## Prerequisites

Ensure that you have the following installed:
- [Node.js](https://nodejs.org/) (>= 14.x)
- [npm](https://www.npmjs.com/) (Node Package Manager) which comes with Node.js
- [MongoDB](https://www.mongodb.com/) (for backend database)

## Setup Instructions

### 1. Backend Setup

1. Navigate to the backend folder:
    ```bash
    cd backend
    ```

2. Install required dependencies:
    ```bash
    npm install axios mongoose nodemon
    ```

3. Start the backend server:
    ```bash
    npm start
    ```

    The backend will now be running locally on the specified port (usually `http://localhost:5000`).

### 2. Frontend Setup

1. After the backend is up and running, navigate to the frontend folder:
    ```bash
    cd ../frontend
    ```

2. Install the required dependencies:
    ```bash
    npm install
    npm install axios
    ```

3. Create the necessary React components using the following code:
    ```javascript
    import { useState } from "react";
    import { useGoogleLogin } from "@react-oauth/google";
    import { googleAuth } from "./api";
    import { useNavigate } from 'react-router-dom';
    import { GoogleOAuthProvider } from "@react-oauth/google";
    import GoogleLogin from './GoogleLogin';
    import { BrowserRouter, Route, Routes, Navigate } from 'react-router-dom';
    ```

4. Start the frontend server:
    ```bash
    npm run dev
    ```

    The frontend will now be running locally (usually at `http://localhost:3000`).

### 3. Verify the Application

- Open your browser and go to the following URLs:
    - Backend: `http://localhost:5000`
    - Frontend: `http://localhost:3000`

## Folder Structure

- **frontend**: Contains the React app and all frontend code.
- **backend**: Contains the Node.js/Express server and the backend code.

## Technologies Used

- **Frontend**: React.js, Axios, Google OAuth
- **Backend**: Node.js, Express.js, Axios, Mongoose, Nodemon
- **Database**: MongoDB

## Acknowledgements

- React, Axios, and other libraries used in the project.
