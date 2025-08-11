# SafeBite  Allergy Management Assistant 🍲

SafeBite is a full-stack web application designed to help users with food allergies manage their condition effectively. It provides tools for tracking symptoms, analyzing ingredient lists for potential allergens using NLP, and generating helpful resources like a "Chef Card" for dining out safely.

---

## ✨ Features

* **User Allergy Profile:** Users can create and manage a detailed profile of their specific allergies and dietary restrictions.
* **Symptom & Exposure Logging:** Easily log food intake and any subsequent symptoms to track patterns over time.
* **AI-Powered Text Analyzer:** Paste an ingredient list or menu description, and the app will use Natural Language Processing to identify potential allergens based on your profile.
* **AI-Enhanced Chef Card:** Automatically generate a clear, concise card for chefs that details your specific allergies and cross-contamination needs.
* **Educational Resources:** Access a database of articles and information about managing allergies.

---

## 🛠️ Tech Stack

* **Frontend:** React, Vite, Tailwind CSS
* **Backend:** Python, Flask
* **Database:** Google Firestore
* **Authentication:** Google Firebase Authentication
* **Natural Language Processing:** spaCy
* **Generative AI:** Google Gemini

---

## 🚀 Getting Started

Follow these instructions to get a local copy up and running for development and testing purposes.

### Prerequisites

* Python 3.9+ and Pip
* Node.js and npm
* A Firebase project with Firestore and Authentication enabled.
* A Google AI Studio API key for Gemini.

### Setup and Installation

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    cd YOUR_REPOSITORY_NAME
    ```

2.  **Backend Setup:**
    * Create a Python virtual environment (e.g., using conda):
        ```sh
        conda create --name safebite_env python=3.10
        conda activate safebite_env
        ```
    * Install Python dependencies:
        ```sh
        pip install -r requirements.txt
        ```
    * Download the spaCy language model:
        ```sh
        python -m spacy download en_core_web_sm
        ```

3.  **Frontend Setup:**
    * Navigate to the frontend directory:
        ```sh
        cd frontend
        ```
    * Install JavaScript dependencies:
        ```sh
        npm install
        ```

4.  **Configuration:**
    * Create a `safebite-firebase-adminsdk.json` file in the `backend/` directory with your Firebase service account key.
    * Create a `firebase_config.js` file in the `frontend/src/` directory with your Firebase web app configuration.
    * Create a `.env` file in the `backend/` directory and add your `GEMINI_API_KEY`.

5.  **Running the Application:**
    * **Start the Backend:** In one terminal, run:
        ```sh
        python backend/app.py
        ```
    * **Start the Frontend:** In a second terminal, run:
        ```sh
        npm run dev
        ```
    * Open your browser and navigate to `http://localhost:5173`.
