# Project Directory Structure

This document outlines the proposed directory structure for the Social Spacefeed application. We will use a monorepo approach to manage our different services.

## Root Directory

The root directory will contain the following:

```
social-spacefeed/
├── docs/
│   ├── architecture.md
│   ├── tech_stack.md
│   ├── api_endpoints.md
│   ├── database_schema.md
│   └── wireframes.md
├── services/
│   ├── ingestion-service/
│   │   ├── src/
│   │   ├── package.json
│   │   └── Dockerfile
│   ├── ai-summarizer/
│   │   ├── src/
│   │   ├── requirements.txt
│   │   └── Dockerfile
│   ├── backend-api/
│   │   ├── src/
│   │   ├── package.json
│   │   └── Dockerfile
│   └── frontend/
│       ├── src/
│       ├── public/
│       ├── package.json
│       └── Dockerfile
├── docker-compose.yml
└── README.md
```

## Directory Descriptions

-   **`docs/`**: This directory will hold all the architecture and planning documents we've created.
-   **`services/`**: This directory will contain the source code for each of our microservices.
    -   **`ingestion-service/`**: The Node.js service for real-time data ingestion.
    -   **`ai-summarizer/`**: The Python service for generating plain-language summaries.
    -   **`backend-api/`**: The Node.js/Express API for the social feed.
    -   **`frontend/`**: The React/Next.js frontend application.
-   **`docker-compose.yml`**: The Docker Compose file to define and run our multi-container application.
-   **`README.md`**: The main README file for the project, containing an overview and setup instructions.

This structure promotes a clean separation of concerns between the different services, while keeping everything in a single, manageable repository.