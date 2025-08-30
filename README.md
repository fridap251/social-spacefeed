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

### 3. Run the Backend

In a new terminal, navigate to the `backend` directory and run the following command:

```bash
npm run dev
```

The backend server will be running on `http://localhost:5000`.

### 4. Run the Frontend

In a new terminal, navigate to the `frontend` directory and run the following command:

```bash
npm start
```

The frontend development server will be running on `http://localhost:3000`. You can open this URL in your web browser to see the Social Spacefeed in action.
