  * EWA – Email Writer Assistant *
-->EWA (Email Writer Assistant) is a lightweight full-stack          application that helps users instantly generate professional email replies based on a topic or short description. Built using React (Vite) for the frontend and Spring Boot for the backend. No database required.

* FEATURES
• Generate professional replies instantly
• Fast Spring Boot backend
• Clean UI with React + Vite
• No database required
• Easy free deployment (Render.com)

* TECH STACK
Frontend: React (Vite), Axios, HTML, CSS, JS
Backend: Java 25, Spring Boot, REST API

* PROJECT STRUCTURE
EWA-Email-Writer-Assistant/
frontend/ # React Vite UI
backend/ # Spring Boot API
README.md # Documentation

* ARCHITECTURE
User sends topic → React UI sends request → Spring Boot generates reply → Response returned to user

* RUN LOCALLY
Backend:
cd backend
./mvnw clean install
./mvnw spring-boot:run

Frontend:
cd frontend
npm install
npm run dev

* API USAGE
Endpoint

POST /api/email/generate

Body:
{
"topic": "Requesting for a meeting schedule"
}

* Frontend Requirements :

• Node.js (v18 or higher)
• NPM (comes automatically with Node.js)

* Backend Requirements :

• Java 25 or Java 21 (LTS versions)
• Maven (no need to install separately because the project includes mvnw wrapper)
->Means users can run Spring Boot with:
./mvnw clean install ./mvnw spring-boot:run
->Required backend dependencies: Spring WebFlux, Lombok, Spring Boot Starter Test, and Reactor Test.


* Deployment
Frontend → Render (Static Site)
Backend → Render (Web Service)

## 🎥 Demo Video

You can watch the demo here:

Google drive : https://drive.google.com/file/d/1VJ8nNKlnkTOpGrToljfdCBcOwtKXr9i_/view?usp=drivesdk

🔌 Extension Feature (AI Reply Button for Gmail)

Along with the main application, we have also created a simple Google Chrome Extension that works as an AI Email Reply helper.
This extension was built by following the basic Chrome extension folder structure and adding our custom popup UI and API call.

The extension can be integrated with Gmail, where it works like an AI Reply Button.
When the user clicks the button, the extension sends the entered topic to our backend and instantly generates a professional reply.

This makes email writing faster and allows users to use our EWA system directly inside Gmail without opening the website.

For this, there is an extension folder is there in main directory from where you can see extension building code.

* AUTHOR
Shravan Kumar Bishnoi - Aspiring Software Engineer
