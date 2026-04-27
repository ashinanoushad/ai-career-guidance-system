# AI Career Guidance System

An AI-powered career guidance web application designed to help students explore career paths, take assessments, and get personalized advice through an intelligent chatbot. Built with a modern full-stack architecture and containerized with Docker.

## Features

- 🤖 **AI Career Chatbot** — Conversational career advisor powered by Google Gemini 2.0 Flash
- 🧠 **Career Assessment** — Questionnaire-based career path recommendation engine
- 🔐 **Facial Recognition Login** — Secure biometric authentication using face recognition and MTCNN
- 👤 **User Dashboard** — Profile management, complaint submission, and facial data management
- 🛡️ **Admin Dashboard** — Manage users, careers, questions, and user complaints
- 🔒 **Session & Role Management** — Role-based access control (Student / Admin)
- 🐳 **Dockerized Deployment** — Full multi-container setup via Docker Compose

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React (Vite), IBM Carbon Design System |
| Backend | Flask, Flask-Sockets (WebSocket) |
| AI / ML | Google Gemini 2.0 Flash, face-recognition, MTCNN, TensorFlow |
| Database | MySQL + SQLAlchemy |
| DevOps | Docker, Docker Compose |

## Getting Started

### Prerequisites
- Docker & Docker Compose installed
- Google Gemini API key

### Run

```bash
git clone https://github.com/ashinanoushad/ai-career-guidance-system.git
cd ai-career-guidance-system
docker compose up --build
```

| Service | URL |
|---|---|
| Frontend | http://localhost:3000 |
| Backend API | http://localhost:5001 |
| MySQL | localhost:3306 |

### Database Setup
Run the provided SQL files to seed initial data:
```bash
# Inside MySQL container or client
source add_careers_query.txt
source add_questions_query.txt
```

## Project Structure

```
├── backend/
│   ├── api/            # Flask routes & WebSocket handlers
│   ├── db/             # SQLAlchemy models & DB config
│   ├── services/       # Business logic (AI, face lock, assessment, user, admin)
│   └── app.py          # App entry point
├── frontend/
│   └── src/
│       ├── components/ # Reusable UI components (AI chatbot widget)
│       ├── pages/      # User & admin pages
│       └── services/   # WebSocket service
└── docker-compose.yml
```
