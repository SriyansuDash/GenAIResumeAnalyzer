# GenAI Resume Analyzer

An intelligent, AI-powered resume analysis tool built with Node.js, Express, MongoDB, and Google's Generative AI (Gemini). This application parses uploaded resumes (PDFs), analyzes their content using advanced language models, and provides actionable feedback, scoring, and insights to help candidates improve their profiles.

## 🚀 Features

*   **PDF Parsing:** Extracts text and data smoothly from uploaded PDF resumes.
*   **AI Analysis:** Utilizes `@google/genai` (Google Gemini) to analyze resume content against industry standards or specific job descriptions.
*   **User Authentication:** Secure user registration and login system with password hashing (`bcrypt`).
*   **Database Integration:** Stores user profiles and previous resume analysis reports using MongoDB and `mongoose`.
*   **RESTful API:** Clean and structured backend API powered by `express`.

## 🛠️ Tech Stack

*   **Runtime:** [Node.js](https://nodejs.org/)
*   **Framework:** [Express.js](https://expressjs.com/)
*   **Database:** [MongoDB](https://www.mongodb.com/) & [Mongoose](https://mongoosejs.com/)
*   **AI Integration:** Google GenAI SDK (`@google/genai`)
*   **Security:** `bcrypt` for password hashing, `cors` for cross-origin requests.
*   **File Processing:** `pdf-parse` / `pdf2json` for handling document uploads.
*   **Development:** `nodemon` for hot-reloading.

## 📋 Prerequisites

Before you begin, ensure you have the following installed:
*   Node.js (v16.x or higher recommended)
*   MongoDB (Local instance or MongoDB Atlas URI)
*   A Google Gemini API Key

## ⚙️ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/GenAIResumeAnalyzer.git
    cd GenAIResumeAnalyzer/backend
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Variables:**
    Create a `.env` file in the `backend` directory and add the following keys:
    ```env
    PORT=5000
    MONGODB_URI=your_mongodb_connection_string
    GEMINI_API_KEY=your_google_gemini_api_key
    JWT_SECRET=your_jwt_secret_key
    ```

4.  **Run the application:**
    *   For development (uses nodemon):
        ```bash
        npm run dev
        ```
    *   For production:
        ```bash
        npm start
        ```

The server should now be running on `http://localhost:3000`.

## 📂 Project Structure

```text
GenAIResumeAnalyzer/
├── backend/
│   ├── node_modules/       # Project dependencies
│   ├── src/                # Source code (Controllers, Routes, Models)
│   ├── .env                # Environment variables
│   ├── .gitignore          # Ignored files for git
│   ├── package.json        # Project metadata and scripts
│   └── package-lock.json   # Dependency lock file
└── frontend/               # Frontend application (if applicable)
```

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! 
Feel free to check the [issues page](https://github.com/your-username/GenAIResumeAnalyzer/issues).

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License.
