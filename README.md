# internship-project
💡 Project Overview

IdeaSpark is a real-time, collaborative web application designed to accelerate the ideation process for teams. It combines the power of synchronous multi-user editing with advanced generative AI to help groups brainstorm efficiently and effectively.

This project is an excellent demonstration of full-stack development skills, showcasing competence in modern UI frameworks, real-time data persistence, and sophisticated API integration.

✨ Key Features

Real-Time Sync: Utilizes Google Firestore to instantly synchronize ideas across all connected users, enabling seamless collaboration.

AI Spark Generator: Integrates the Gemini API (gemini-2.5-flash-preview-09-2025) to generate three unique, context-aware ideas based on the current board's topic and existing entries.

Secure & Anonymous Access: Employs Firebase Authentication for quick, token-based user identification without requiring a login, making the app instantly accessible.

Responsive Design: Built with React and styled using Tailwind CSS for a clean, modular, and fully responsive interface on all devices.

🛠️ Technology Stack

Category

Technology

Purpose

Frontend

React

Component-based UI development.

Styling

Tailwind CSS

Utility-first, responsive design framework.

Real-time DB

Google Firestore

Persistent, real-time data synchronization.

Authentication

Firebase Auth

User identification and session management.

AI/ML

Gemini API

Generative AI for idea generation.

🚀 Installation & Local Setup

To run IdeaSpark locally, follow these steps:

1. Prerequisites

You must have Node.js (LTS recommended) and npm installed.

2. Project Setup

Use Vite to initialize a new React project and navigate into the directory:

# Create project (choose React and JavaScript)
npm create vite@latest ideaspark-project -- --template react
cd ideaspark-project
npm install


3. Install Dependencies

Install the necessary libraries for Firebase and Tailwind:

# Install Firebase SDK
npm install firebase

# Install Tailwind CSS and its dependencies
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p


(Note: Ensure your tailwind.config.js is configured to scan your source files, as shown in the provided file.)

4. Configuration

Replace the placeholder configuration at the top of the src/App.jsx file with your own:

Firebase Config: Obtain your apiKey, projectId, etc., from the Firebase Console.

Gemini API Key: Obtain your key from the Google AI Studio.

const firebaseConfig = { /* ... your Firebase details ... */ };
const API_KEY = "YOUR_GEMINI_API_KEY";


5. Run the Application
