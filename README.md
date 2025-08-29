# Social Spacefeed

This is the monorepo for the Social Spacefeed application.

## Prerequisites

Before you begin, ensure you have the following installed:

-   [Node.js](https://nodejs.org/) (which includes npm)
-   [Python](https://www.python.org/)
-   [MongoDB](https://www.mongodb.com/try/download/community)

## Running the Application

This project is a monorepo that uses npm workspaces.

### 1. Install Dependencies

First, install all the dependencies for the `backend` and `frontend` workspaces from the root of the project:

```bash
npm install
```

### 2. Start MongoDB

Ensure your MongoDB server is running.

### 3. Run the Application

You can run both the backend and frontend concurrently with a single command from the root of the project:

```bash
npm run dev
```

This will:

-   Start the backend server in development mode.
-   Start the frontend development server.

The frontend will be available at `http://localhost:3000`, and the backend will be running on the port specified in its environment variables (e.g., `http://localhost:3001`).
