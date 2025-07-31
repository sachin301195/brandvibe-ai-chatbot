# 🤖 BrandVibe AI Chatbot

A submission for the Olivia AI "Vibe Coder" coding challenge. BrandVibe AI is a creative partner designed to help founders, marketers, and designers craft compelling prompts for generating on-brand content.

**https://brandvibe-ai-chatbot.vercel.app/**

---

## The "Vibe" (The Product)

In a world full of generic AI tools, **BrandVibe AI** was built on a specific insight: creativity needs context. This chatbot doesn't just give answers; it acts as a specialized creative strategist.

Instead of taking a vague idea, it asks targeted questions about brand voice, visual style, and target audience to help the user build a highly effective, detailed prompt. It's a "meta" AI tool designed to improve a user's interaction with other powerful generative models, ensuring the output is always on-brand. This concept was inspired by my experience as an LLM Trainer, where I learned that a well-crafted prompt is the key to unlocking an AI's true potential.

## Key Features ✨

-   **Conversational UI:** A sleek, responsive, and dark-themed chat interface built with React and TypeScript.
-   **Live Gemini Integration:** Fully functional integration with Google's `gemini-1.5-flash-latest` model for real-time, contextual conversations.
-   **Secure API Key Management:** A clean, user-friendly modal allows users to securely save their Google AI API key to their browser's `localStorage`.
-   **Markdown Rendering:** Correctly parses and displays Markdown in the AI's responses for enhanced readability.
-   **UX Polishing:** Includes a "typing" indicator to provide feedback during API calls, ensuring a smooth user experience.

## Tech Stack

-   **Frontend:** React, TypeScript, Vite
-   **Styling:** CSS Modules
-   **AI Integration:** Google Generative AI SDK (`@google/generative-ai`)
-   **Version Control:** Git & GitHub

## My "Vibe Coder" Process

This project was built using an **AI-native development process**, leveraging an AI co-pilot as a true partner from the first line of code to the final bug fix. My AI chat history is the most important deliverable, as it showcases a modern, high-velocity workflow.

The process was iterative and focused:
1.  **Ideation:** Brainstorming a unique chatbot persona that aligned with my background as an LLM Trainer.
2.  **Scaffolding:** Using the AI to generate the initial project structure, components, and styling.
3.  **Iterative Debugging:** Collaborating with the AI to solve problems. A key moment was debugging a stubborn CSS layout issue where `margin: 0 auto` wasn't working. By describing the problem to the AI ("the parent is likely a flex container"), we quickly identified and fixed a conflicting global style in `index.css`.
4.  **Implementation:** Prompting the AI to implement core features like the API key modal and the final Gemini API integration, focusing on best practices like using official SDKs.

This method allowed for rapid development while I focused on the higher-level product vision, architecture, and user experience.

## How to Run Locally

1.  Clone the repository:
    ```bash
    git clone https://github.com/sachin301195/brandvibe-ai-chatbot.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd brandvibe-ai-chatbot
    ```
3.  Install dependencies:
    ```bash
    npm install
    ```
4.  Run the development server:
    ```bash
    npm run dev
    ```
5.  Open your browser to `http://localhost:5173`.
6.  Click the settings icon, enter your Google AI API key, and start chatting!