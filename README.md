# EduReach-Agentic-College-Chatbot

[![React](https://img.shields.io/badge/React-19.1.0-blue?logo=react)](https://reactjs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-blue?logo=typescript)](https://www.typescriptlang.org)
[![Node.js](https://img.shields.io/badge/Node.js-24.x-green?logo=node.js)](https://nodejs.org)
[![Express](https://img.shields.io/badge/Express-5.2-black?logo=express)](https://expressjs.com)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-green?logo=mongodb)](https://www.mongodb.com)
[![LangChain](https://img.shields.io/badge/LangChain-1.2.26-blue?logo=langchain)](https://langchain.com)
[![Google Gemini](https://img.shields.io/badge/Google%20Gemini-2.5%20Flash-blue?logo=google)](https://cloud.google.com/generative-ai)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

## Project Overview

EduReach-Agentic-College-Chatbot is an open-source AI-powered college guidance assistant. The platform combines a React front end, a TypeScript-powered Node.js and Express backend, and MongoDB Atlas for persistence. It is designed to support an agentic chatbot experience through a Retrieval-Augmented Generation (RAG) architecture.

## Features

- AI College Chatbot
- Agentic AI architecture
- LangChain integration
- Google Gemini support
- MongoDB Atlas Vector Search
- RAG (Retrieval-Augmented Generation)
- JWT authentication
- Login & signup flows
- Responsive UI
- Knowledge base search
- Protected routes
- Modern React interface

## Tech Stack

### Frontend
- React
- TypeScript
- Vite
- Tailwind CSS
- React Router
- Axios
- React Hot Toast

### Backend
- Node.js
- Express.js
- TypeScript
- JWT
- bcryptjs
- Mongoose

### Database
- MongoDB Atlas
- MongoDB Vector Search

### AI Technologies
- LangChain
- Google Gemini
- RAG architecture
- Embeddings
- Retriever workflows

### Deployment
- Vercel (frontend)
- Render / Railway (backend)
- MongoDB Atlas

## Architecture

EduReach is structured as an API-driven full stack application with a focus on intelligent retrieval.

User
↓
React Frontend
↓
Express Backend
↓
LangChain Agent
↓
Retriever Tool
↓
MongoDB Atlas Vector Search
↓
Knowledge Base
↓
Gemini 2.5 Flash
↓
Final AI Response

## Folder Structure

```
.
├── .gitignore
├── .env.example
├── API_DOCUMENTATION.md
├── ARCHITECTURE.md
├── AI_WORKFLOW.md
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── DEPLOYMENT.md
├── INSTALLATION.md
├── LICENSE
├── PROJECT_STRUCTURE.md
├── README.md
├── SECURITY.md
├── edureach-platform
│   ├── client
│   │   ├── package.json
│   │   ├── tsconfig.json
│   │   ├── tsconfig.app.json
│   │   ├── vite.config.ts
│   │   ├── public
│   │   └── src
│   └── server
│       ├── package.json
│       ├── tsconfig.json
│       ├── src
│       │   ├── app.ts
│       │   ├── server.ts
│       │   ├── config
│       │   ├── controllers
│       │   ├── middleware
│       │   ├── models
│       │   ├── routes
│       │   └── utils
│       └── knowledge-base
└── thunder-tests
```

## Installation Guide

### Clone repository
```bash
git clone <repository-url>
cd Projects
```

### Install frontend
```bash
cd edureach-platform/client
npm install
```

### Install backend
```bash
cd ../server
npm install
```

### Environment setup
Copy `.env.example` to `.env` and add your configuration values.

### Run frontend
```bash
cd edureach-platform/client
npm run dev
```

### Run backend
```bash
cd edureach-platform/server
npm run dev
```

## Environment Variables

- `PORT` — Backend server port.
- `MONGODB_URI` — MongoDB Atlas connection string.
- `JWT_SECRET` — Secret for signing JWT tokens.
- `JWT_EXPIRES_IN` — Expiration time for JWT tokens.
- `CLIENT_URL` — Frontend origin for CORS.
- `GOOGLE_API_KEY` — Google API key for Gemini.

## API Endpoints

### POST /api/auth/register
Register a new user.

### POST /api/auth/login
Authenticate and return a JWT.

### GET /api/auth/me
Retrieve the current authenticated user.

### POST /api/chat/message (planned)
Send a prompt to the AI chatbot and return a generated response.

## RAG Pipeline

- Load knowledge documents.
- Split content into embeddings-ready chunks.
- Embed text using a vector model.
- Store vectors in MongoDB Atlas.
- Retrieve relevant context for each query.
- Generate the final response with Gemini.

## AI Technologies Used

### LangChain
Used for orchestrating retrieval and agent workflows.

### Google Gemini
Targeted LLM for response generation.

### MongoDB Atlas
Data persistence and vector search support.

### Vector Search
Enables semantic retrieval from the knowledge base.

### Embeddings
Convert text into vectors for similarity search.

### Agentic AI
Integrates retrieval tools with language generation to create context-aware answers.

## Screenshots

### Home Page
![Home Page](docs/screenshots/home.png)

### Login
![Login](docs/screenshots/login.png)

### Signup
![Signup](docs/screenshots/signup.png)

### Chat
![Chat](docs/screenshots/chat.png)

### Mobile View
![Mobile View](docs/screenshots/mobile.png)

## Future Improvements

- Voice agent support
- WhatsApp integration
- PDF knowledge upload
- Admin dashboard
- Analytics
- Multi-language support

## Contributing

See `CONTRIBUTING.md`.

## License

MIT License

## Author

EduReach-Agentic-College-Chatbot maintainers.

