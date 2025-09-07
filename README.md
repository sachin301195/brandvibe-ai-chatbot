# BrandVibe: A Full-Stack AI Chatbot Application

**Live Demo:** [https://brandvibe-ai-chatbot.vercel.app/](https://brandvibe-ai-chatbot.vercel.app/)

## 1. Problem Statement

This project is a demonstration of full-stack application development, showcasing the integration of a modern frontend, a secure API backend, and a third-party AI service. The objective was to build a responsive, real-time conversational AI application from the ground up, focusing on clean architecture, state management, and user experience.

The application, originally developed as a technical assessment, serves as a practical portfolio piece for demonstrating skills in API integration, frontend development with React, and secure client-side secret management.

## 2. Tech Stack & Architecture

This project utilizes a modern, robust tech stack to deliver a seamless user experience.

* **Frontend:** React, TypeScript, Vite
* **Styling:** CSS Modules
* **API Integration:** Google Generative AI SDK (`@google/generative-ai`) for connecting to the Gemini 1.5 Flash model.
* **Version Control:** Git & GitHub
* **Deployment:** Vercel

### Architecture Overview

The application follows a classic client-server architecture:

1.  **Client-Side (React UI):** A responsive single-page application (SPA) built with React and TypeScript provides the user interface. It manages the chat history state, handles user input, and displays the conversation in real-time.
2.  **API Key Management:** To ensure security, the user's Google AI API key is managed exclusively on the client-side using the browser's `localStorage`. This prevents the key from being exposed in the codebase or network logs.
3.  **Gemini API:** The frontend communicates directly with the Google Generative AI API, sending the conversation history and new user prompts to the `gemini-1.5-flash-latest` model for processing.
4.  **Deployment:** The application is deployed on Vercel, demonstrating a streamlined CI/CD workflow for frontend applications.

## 3. Key Features & Implementation Details

### Secure API Key Management
A key feature is the secure handling of user credentials.
* A user-friendly modal allows users to input their Google AI API key.
* The key is stored securely in the browser's `localStorage` and is never exposed in the source code, adhering to security best practices.

### Real-Time Conversational UI
The user interface is designed for a modern chat experience.
* Built with **React and TypeScript**, ensuring a type-safe and maintainable codebase.
* Includes a "typing" indicator to provide clear visual feedback to the user while waiting for the AI's response, enhancing the user experience.
* The UI correctly renders Markdown in the AI's responses for better readability of formatted text like lists or code blocks.

## 4. How to Run Locally

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/sachin301195/brandvibe-ai-chatbot.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd brandvibe-ai-chatbot
    ```
3.  **Install dependencies:**
    ```bash
    npm install
    ```
4.  **Run the development server:**
    ```bash
    npm run dev
    ```
5.  Open your browser to `http://localhost:5173`.
6.  Click the settings icon, enter your own Google AI API key, and begin the conversation.
