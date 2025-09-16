# Weather-App

This is a full-stack weather application built using the MERN stack (MongoDB, Express.js, React, Node.js). It features user authentication (signup and login) and a weather dashboard that displays real-time weather information for a specified city or the user's current location.

## Features

-   **User Authentication**: Secure user registration and login functionalities are implemented using `bcryptjs` for password hashing.
-   **MongoDB Database**: User data is stored in a MongoDB database, with `mongoose` serving as the ODM (Object Data Modeling) library.
-   **RESTful API**: The backend is built with `Express.js`, providing API endpoints for user signup and login.
-   **Dynamic Weather Display**: Users can search for weather information by city name or use their browser's geolocation feature.
-   **Responsive UI**: The client-side interface is styled with Tailwind CSS and is designed to be responsive.

## Screenshots

<img width="1695" height="865" alt="Screenshot 2025-08-20 212753" src="https://github.com/user-attachments/assets/657f2785-405a-469b-90dd-f34fa9167186" />

<img width="1407" height="897" alt="Screenshot 2025-08-20 212443" src="https://github.com/user-attachments/assets/7a9b9ae1-508d-4ac2-ab4e-3bd584528247" />

## Technologies Used

* **Frontend**:
    * HTML, CSS (`style.css`), JavaScript (`client.js`)
    * Tailwind CSS for styling
    * OpenWeatherMap API for weather data
* **Backend**:
    * Node.js and Express.js
    * MongoDB with Mongoose
    * bcryptjs for password hashing
    * cors for enabling Cross-Origin Resource Sharing

## Prerequisites

-   Node.js (version 22.18.0 or later recommended)
-   MongoDB installed and running on `mongodb://127.0.0.1:27017`

## Installation and Setup

1.  **Clone the repository:**
    ```sh
    git clone <repository_url>
    cd MERN-PROJECT-1
    ```

2.  **Install dependencies:**
    ```sh
    npm install
    ```

3.  **Set up MongoDB:**
    Ensure your MongoDB server is running. The application connects to a database named `weather-auth-app` at `mongodb://127.0.0.1:27017`.

4.  **Start the server:**
    ```sh
    npm start
    ```
    This will start the Express.js server, and you should see the message "Server is running on http://localhost:3000" in your console.

5.  **Access the application:**
    Open your web browser and navigate to `http://localhost:3000`.

## API Endpoints

-   `POST /api/signup`: Registers a new user. Expects a JSON body with `email` and `password`.
-   `POST /api/login`: Authenticates a user. Expects a JSON body with `email` and `password`.
