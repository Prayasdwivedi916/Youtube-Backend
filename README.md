# YouTube Backend

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Usage](#usage)
6. [API Endpoints](#api-endpoints)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction
The YouTube Backend project is a comprehensive backend system built using the MERN stack (MongoDB, Express.js, React.js, and Node.js). This backend supports core functionalities required for a video-sharing platform like YouTube, including user management, video uploads, and video streaming.

## Features
- **User Authentication**: Secure user registration and login using JWT.
- **Video Management**: Upload, update, and delete videos.
- **Video Streaming**: Efficient video streaming capabilities.
- **Comments and Ratings**: Users can comment on and rate videos.
- **Search Functionality**: Powerful search to find videos by title, description, or tags.
- **Playlists**: Create and manage video playlists.
- **Subscriptions**: Subscribe to channels and get updates.

## Technologies Used
- **Frontend**: React.js, Redux
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)
- **Other Tools**: Mongoose, Multer (for file uploads), Bcrypt.js

## Installation
Follow these steps to install and set up the project locally:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Prayasdwivedi916/YouTube-Backend.git
   cd YouTube-Backend
   ```

2. **Install server dependencies:**
   ```bash
   cd server
   npm install
   ```

3. **Install client dependencies:**
   ```bash
   cd ../client
   npm install
   ```

4. **Set up environment variables:**
   Create a `.env` file in the `server` directory and add the following:
   ```plaintext
   MONGO_URI=your_mongo_database_uri
   JWT_SECRET=your_jwt_secret
   ```

5. **Start the server and client:**
   ```bash
   # In the server directory
   npm start

   # In the client directory
   npm start
   ```

6. **Access the application:**
   Open your browser and navigate to `http://localhost:3000`.

## Usage
- **Admin Panel**: Manage users, videos, and overall platform settings.
- **User Dashboard**: Upload and manage your own videos, view subscriptions, and interact with the community.

## API Endpoints
Here are some of the key API endpoints available:

- **User Authentication**
  - `POST /api/auth/register`: Register a new user.
  - `POST /api/auth/login`: Login an existing user.

- **Videos**
  - `POST /api/videos/upload`: Upload a new video.
  - `GET /api/videos`: Get all videos.
  - `GET /api/videos/:id`: Get a specific video.
  - `PUT /api/videos/:id`: Update a specific video.
  - `DELETE /api/videos/:id`: Delete a specific video.

- **Comments**
  - `POST /api/comments`: Add a comment to a video.
  - `GET /api/comments/:videoId`: Get all comments for a specific video.

- **Ratings**
  - `POST /api/ratings`: Rate a video.

- **Playlists**
  - `POST /api/playlists`: Create a new playlist.
  - `GET /api/playlists`: Get all playlists.
  - `PUT /api/playlists/:id`: Update a specific playlist.
  - `DELETE /api/playlists/:id`: Delete a specific playlist.

- **Subscriptions**
  - `POST /api/subscriptions`: Subscribe to a channel.
  - `GET /api/subscriptions`: Get all subscriptions for a user.

## Contributing
Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a pull request.

Feel free to adjust any sections or add more details as per your project specifics.
