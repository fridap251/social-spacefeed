# URL and Port Mappings

This document provides a visual guide to the URLs and ports used by each service in the Social Spacefeed application when running locally.

## URL Diagram

```mermaid
graph TD
    subgraph "User's Browser"
        A[http://localhost:3002] --> B{Frontend}
    end

    subgraph "Services"
        B -- "Socket.IO" --> C(Ingestion Service\nhttp://localhost:3000)
        B -- "REST API" --> D(Backend API\nhttp://localhost:3001)
        E(AI Summarizer) -- "Socket.IO" --> C
        E -- "REST API" --> D
    end

    subgraph "Database"
        D -- "Mongoose" --> F[(MongoDB\nlocalhost:27017)]
    end
```

## Service URLs

-   **Frontend:** `http://localhost:3002`
    -   This is the URL you will open in your web browser to use the Social Spacefeed application.

-   **Ingestion Service:** `http://localhost:3000`
    -   This service provides a WebSocket connection for real-time data streaming. The frontend and AI summarizer connect to this URL.

-   **Backend API:** `http://localhost:3001`
    -   This service provides the REST API for posts, likes, and comments. The frontend and AI summarizer connect to this URL.

-   **MongoDB:** `localhost:27017`
    -   This is the default port for the MongoDB database. The Backend API connects to this to store and retrieve data.