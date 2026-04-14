🚀 AI-Assisted Career Guidance System

📌 Overview

The AI-Assisted Career Guidance System is a full-stack web application that recommends suitable career paths based on user responses to a structured questionnaire.

The system combines:

Generative AI (Google Gemini API) for reasoning
Rule-based validation for reliability

Unlike typical AI systems, this project ensures that the output is validated and controlled, making it more dependable for real-world usage.

🎯 Objective

To help users make informed career decisions by:

Analyzing responses to 30 structured questions
Generating AI-based career recommendations
Ensuring output validity using a predefined dataset

🧠 System Workflow


User answers 30 questions
Responses are sent to the backend
Backend constructs a structured prompt
Prompt is sent to Google Gemini API
Gemini generates a career recommendation
System validates output against career dataset
If valid → displayed to user
If invalid → system re-prompts AI
⚙️ Architecture
Frontend (React) → Handles user interaction
Backend (Flask) → Processes logic and API calls
AI Layer (Gemini API) → Generates recommendations
Database (MySQL) → Stores career dataset

👉 The system follows a client-server architecture with a clear separation of concerns.


🎯 Key Features


✅ AI-assisted career recommendation
✅ Prompt engineering for controlled AI output
✅ Validation layer for accuracy
✅ Interactive user interface
✅ Backend service-based structure
✅ AI chatbot for additional guidance
🛠️ Tech Stack
Frontend
React.js
HTML, CSS, JavaScript
Backend
Flask (Python)
REST APIs
AI Integration
Google Gemini API
Database
MySQL
Deployment
Docker & Docker Compose


📂 Project Structure

backend/    → API routes, services, AI integration, validation  
frontend/   → User interface (React components)  
database/   → SQL scripts and dataset  
⚙️ Setup Instructions
1. Clone the repository
git clone https://github.com/ashinanoushad/ai-career-guidance-system.git
cd ai-career-guidance-system
2. Install dependencies
npm install
3. Run the project
npm start


🧪 Core Concepts Used

Prompt Engineering
REST API Design
Client-Server Architecture
Validation Logic
AI + Rule-Based Hybrid System


⚠️ Limitations

Depends on external AI (Gemini API)
Output quality depends on prompt design
May require multiple attempts for valid results


🚀 Future Improvements

Improve prompt accuracy
Add user authentication
Store user history
Provide multiple career suggestions
Integrate custom ML model


👩‍💻 Author

Ashina Noushad
