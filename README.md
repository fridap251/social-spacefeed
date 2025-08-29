# Social Spacefeed

Social Spacefeed is a social application designed to stream mission telemetry data in real-time. The platform leverages AI to generate summaries and visuals, enhancing user engagement and understanding of the telemetry information.

## Features

- **Live Telemetry Feed**: Stream real-time telemetry data from missions.
- **AI-Generated Summaries**: Automatically generated summaries of telemetry data for quick insights.
- **Visual Representations**: Visuals created from telemetry data to aid in understanding complex information.
- **User Interaction**: Like and comment functionality to engage with the content.

## Project Structure

The project is organized into three main directories: `backend`, `frontend`, and `shared`.

- **backend**: Contains the server-side code, including API routes, controllers, services, and database management.
- **frontend**: Contains the client-side code, built with React, for rendering the user interface and handling user interactions.
- **shared**: Contains shared types and utility functions used across both backend and frontend.

## Getting Started

### Prerequisites

- Node.js
- npm or pnpm
- Docker (for containerized setup)

### Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd social-spacefeed
   ```

2. Install dependencies for both backend and frontend:
   ```
   cd backend
   npm install
   cd ../frontend
   npm install
   ```

3. Set up environment variables:
   - Copy the `.env.example` files in both `backend` and `frontend` to `.env` and fill in the required values.

### Running the Application

To run the application in development mode:

1. Start the backend server:
   ```
   cd backend
   npm run dev
   ```

2. Start the frontend application:
   ```
   cd frontend
   npm start
   ```

### Docker Setup

To run the application using Docker, use the following command:
```
docker-compose up
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.