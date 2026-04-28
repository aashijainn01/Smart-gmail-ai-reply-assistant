🚀 Smart Email Generator (Full Stack GenAI Application)

📌 Overview
Smart Email Generator is a full-stack AI-powered application that generates professional, context-aware emails based on user input.
It integrates a React frontend with a Spring Boot backend, which communicates with Generative AI APIs (Gemini / OpenAI / Ollama) to generate high-quality email content in real time.
This project demonstrates real-world AI integration, REST API design, and full-stack development, making it highly relevant for GenAI + Backend + Full Stack roles.


✨ Features
🧠 AI-powered email generation
🎯 Custom inputs (purpose, tone, recipient)
⚡ Instant email generation via REST API
🔄 Regenerate email option
🌐 Full-stack architecture (React + Spring Boot)
🔌 AI API integration (Gemini / OpenAI / Ollama)
💻 Clean and responsive UI (Vite + React)


🛠️ Tech Stack
💻 Frontend
React.js (Vite)
HTML, CSS, JavaScript
⚙️ Backend
Java
Spring Boot
REST APIs
Maven
🤖 AI Integration
Gemini API / OpenAI API
Ollama (Local AI for offline usage)


🏗️ Project Architecture
React Frontend (email-writer-react)
        ↓
Spring Boot Backend (email-writer-sb)
        ↓
Service Layer (EmailGeneratorService)
        ↓
AI API (Gemini / OpenAI / Ollama)
        ↓
Generated Email Response
        ↓
Frontend Display


📂 Project Structure
email-writer-sh/
│
├── email-writer-react/        # Frontend (React + Vite)
│   ├── src/
│   ├── public/
│   ├── index.html
│   └── package.json
│
├── email-writer-sb/           # Backend (Spring Boot)
│   ├── src/main/java/com/email/email_writer/
│   │   ├── EmailWriterSbApplication.java
│   │   └── writer/app/
│   │       ├── EmailGeneratorController.java
│   │       ├── EmailGeneratorService.java
│   │       └── EmailRequest.java
│   │
│   ├── resources/
│   └── pom.xml
│
└── README.md


⚙️ How It Works
User enters email details in React UI
Frontend sends POST request to backend
Spring Boot processes request via controller
Service layer builds AI prompt
AI API generates email content
Response is returned and displayed instantly


🔗 API Endpoint
Generate Email
POST /api/email/generate
Request Body
{
  "purpose": "Job Application",
  "tone": "Professional",
  "recipient": "Hiring Manager"
}
Response
{
  "emailContent": "Dear Hiring Manager, ..."
}


⚡ Setup & Installation
🔽 Clone Repository
git clone https://github.com/your-username/email-writer-sh.git
cd email-writer-sh

🖥️ Backend Setup (Spring Boot)
cd email-writer-sb
mvn spring-boot:run

Runs on:
http://localhost:8080

🌐 Frontend Setup (React)
cd email-writer-react
npm install
npm run dev

Runs on:
http://localhost:5173


🔑 AI Configuration
In application.properties:
ai.api.key=YOUR_API_KEY

👉 For Ollama (free & offline):
No API key required, just run:
ollama run llama3


🔥 Core Backend Logic
String prompt = "Write a " + tone + " email for " + purpose;
String response = aiService.generateEmail(prompt);
🚀 Future Enhancements
📧 Send email via SMTP / Gmail API
🎙️ Voice-based email generation
🌍 Multi-language support
📂 Save & edit drafts
🤖 Fine-tuned AI responses


💡 Use Cases
Job applications
Professional emails
Cold outreach
Customer support replies
Business communication

📊 Why This Project is Strong
✅ Real-world GenAI integration
✅ Full-stack architecture
✅ REST API design
✅ Scalable backend structure
✅ Production-ready concept


👩‍💻 Author
Aashi Jain
Java Backend AI Developer
