# Social Spacefeed

This is the monorepo for the Social Spacefeed application.

## Prerequisites

Before you begin, ensure you have the following installed:

-   [Node.js](https://nodejs.org/) (which includes npm)
-   [Python](https://www.python.org/)
-   [MongoDB](https://www.mongodb.com/try/download/community)

## Running the Application

To run the application, you will need to open four separate terminals and run each service individually.

### 1. Start MongoDB

Ensure your MongoDB server is running.

### 2. Start the Backend API

In a new terminal, navigate to the `backend-api` directory and run the following commands:

```bash
cd services/backend-api
npm install
npm start
```

The backend API will be running on `http://localhost:3001`.

### 3. Start the Ingestion Service

In a new terminal, navigate to the `ingestion-service` directory and run the following commands:

```bash
cd services/ingestion-service
npm install
npm start
```

The ingestion service will be running on `http://localhost:3000`.

### 4. Start the AI Summarizer

In a new terminal, navigate to the `ai-summarizer` directory and run the following commands:

```bash
cd services/ai-summarizer
pip install -r requirements.txt
python src/main.py
```

The AI summarizer will connect to the ingestion service and the backend API.

### 5. Start the Frontend

In a new terminal, navigate to the `frontend` directory and run the following commands:

```bash
cd services/frontend
npm install
npm run dev
```

The frontend development server will be running on `http://localhost:3002`. You can open this URL in your web browser to see the Social Spacefeed in action.
