✉️ AI Gmail Reply Assistant

🚀 AI Gmail Reply Assistant is a Chrome Extension that generates context-aware email replies automatically using Generative AI.

The extension integrates directly into the Gmail interface and allows users to generate smart email responses with one click.

This project demonstrates Chrome Extension development, Gmail DOM manipulation, and backend AI integration using Spring Boot.

🚀 Features

✅ Generate AI-powered email replies instantly
✅ Works directly inside Gmail as a Chrome Extension
✅ Extracts email context automatically
✅ One-click AI reply generation
✅ Spring Boot backend for AI processing
✅ Clean and lightweight integration with Gmail

🛠 Tech Stack
Frontend

🟨 JavaScript

🌐 HTML

🎨 CSS

🧩 Chrome Extension APIs (Manifest V3)

📧 Gmail DOM Manipulation

Backend

☕ Java

🌱 Spring Boot

🔗 REST APIs

AI Integration

🤖 Generative AI API (Gemini / Ollama / Claude depending on your setup)

🏗 Architecture
Gmail Interface
      │
      ▼
Chrome Extension (content.js)
      │
      ▼
Spring Boot Backend API
      │
      ▼
Generative AI Model
      │
      ▼
Generated Email Reply

The Chrome Extension extracts the email content from Gmail, sends it to the backend API where the AI model generates a reply, and the response is inserted back into Gmail.

⚙️ How It Works

1️⃣ User opens an email in Gmail
2️⃣ The extension injects an AI Reply button into the Gmail interface
3️⃣ When clicked:

The extension extracts the email text

Sends it to the Spring Boot backend

4️⃣ The backend calls the Generative AI API
5️⃣ AI generates a context-aware email reply
6️⃣ The reply is inserted into the Gmail compose box

📂 Project Structure
ai-email-assistant-extension
│
├── extension
│   ├── manifest.json
│   ├── content.js
│   ├── content.css
│
├── backend
│   ├── controller
│   ├── service
│   └── Application.java
│
└── README.md
💻 Installation Guide
1️⃣ Clone the Repository
git clone https://github.com/aashijainn01/ai-email-assistant-extension.git
2️⃣ Setup Backend (Spring Boot)

Navigate to backend folder

cd backend

Run the Spring Boot application

mvn spring-boot:run

Backend runs at:

http://localhost:8080
3️⃣ Load Chrome Extension

Open Google Chrome

Go to:

chrome://extensions

Enable Developer Mode

Click Load Unpacked

Select the extension folder

The extension will now be installed.

📖 Usage

1️⃣ Open Gmail
2️⃣ Open any email thread
3️⃣ Click the AI Reply button
4️⃣ AI will generate a reply automatically
5️⃣ Edit if necessary and send

🎯 Example Use Cases

📧 Quickly draft professional email replies
📧 Save time responding to emails
📧 Improve email writing productivity
📧 Generate structured responses for work or communication

🧠 Key Technical Highlights

⭐ Chrome Extension built using Manifest V3
⭐ Gmail DOM manipulation to inject custom UI
⭐ Client-Server architecture using REST APIs
⭐ Integration with Generative AI APIs
⭐ Real-time email reply generation

🔮 Future Improvements

🚀 Email tone selection (Formal / Casual / Friendly)
🚀 Email summarization feature
🚀 Multi-language reply generation
🚀 Support for multiple email platforms
🚀 Deploy backend to cloud (AWS / Render / Railway)

📚 Learning Outcomes

Through this project I learned:

✔ Chrome Extension development
✔ Gmail DOM manipulation
✔ Backend API development using Spring Boot
✔ Integration with Generative AI models
✔ Asynchronous API communication

📜 License

This project is licensed under the MIT License.
