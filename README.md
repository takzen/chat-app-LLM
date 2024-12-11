# AI Chat Application

## Overview
This project is a full-stack AI Chat application that provides an intuitive interface for users to interact with AI-powered chats. The system supports creating, retrieving, and managing chat histories and is built using a modern tech stack.

### Key Features
- **Frontend**:
  - A responsive and user-friendly UI for managing and interacting with chats.
  - Integration with AI to handle user queries.
  - Secure authentication with Clerk.
- **Backend**:
  - RESTful API for managing chat data and images.
  - Image upload and management using ImageKit.
  - MongoDB for data storage.

## Technologies Used

### Frontend
- **Framework**: React with Vite for fast development and build processes.
- **Routing**: React Router DOM for client-side routing.
- **State Management**: React Context for managing chat states.
- **Animations**: React Type Animation for dynamic typing effects.
- **API Integration**: Google Generative AI SDK.

### Backend
- **Framework**: Express.js for RESTful APIs.
- **Database**: MongoDB with Mongoose for schema-based data modeling.
- **Image Management**: ImageKit for handling image uploads.
- **Environment Variables**: dotenv for secure configuration management.
- **Authentication**: Clerk SDK for user management and authentication.

## Getting Started

### Prerequisites
Ensure the following tools are installed:
- Node.js (v18 or higher)
- npm or yarn
- MongoDB instance (local or cloud-based)
- ImageKit account for image handling

### Frontend Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```
3. Run the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```
4. Open [http://localhost:5173](http://localhost:5173) in your browser.

### Backend Setup
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Create a `.env` file based on the provided `.env.example`:
   ```env
   MONGO=mongodb+srv://<username>:<password>@cluster0.mongodb.net/chatdb
   CLIENT_URL=http://localhost:5173
   IMAGE_KIT_ENDPOINT=<your-imagekit-endpoint>
   IMAGE_KIT_PUBLIC_KEY=<your-imagekit-public-key>
   IMAGE_KIT_PRIVATE_KEY=<your-imagekit-private-key>
   PORT=3000
   ```
3. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```
4. Run the development server:
   ```bash
   npm start
   ```
5. Ensure the backend is running at [http://localhost:3000](http://localhost:3000).

## Project Structure

### Frontend
- `src/routes/`: Contains individual pages for the application.
- `src/layouts/`: Layout components for consistent UI structure.
- `src/context/`: Manages global states for the chat application.

### Backend
- `models/`: MongoDB schemas for chat and user chat data.
- `routes/`: API routes for handling chat and image-related operations.
- `index.js`: Entry point for the Express server.

## Available Scripts

### Frontend Scripts
- `npm run dev`: Starts the development server.
- `npm run build`: Builds the application for production.
- `npm run lint`: Lints the codebase using ESLint.
- `npm run preview`: Previews the production build.

### Backend Scripts
- `npm start`: Starts the backend server with nodemon.
- `npm test`: Placeholder for future tests.

## Live Demo
You can view the live demo [here](#) (provide the URL if available).

## License
This project is licensed under the [MIT License](LICENSE).
