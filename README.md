# AMBIGAPATHY'S-RAG-CHATBOT (RAG Project - Backend & Frontend)


This repository contains both the backend and frontend implementations for the RAG (Retrieval-Augmented Generation) project. The backend is built using Python, and the frontend is built using Next.js. The backend handles tasks like web scraping, embeddings, and chat functionalities, while the frontend renders the user interface and interacts with the backend API.

---

## Table of Contents

1. [Backend Setup](#backend-setup)
    - [Project Structure](#backend-project-structure)
    - [Requirements](#backend-requirements)
    - [Setup](#backend-setup-steps)
    - [Usage](#backend-usage)
2. [Frontend Setup](#frontend-setup)
    - [Project Structure](#frontend-project-structure)
    - [Requirements](#frontend-requirements)
    - [Setup](#frontend-setup-steps)
    - [Usage](#frontend-usage)
3. [Project Workflow](#project-workflow)
    - [Backend Workflow](#backend-workflow)
    - [Frontend Workflow](#frontend-workflow)
4. [License](#license)

---

## Backend Setup

### Backend Project Structure

The backend directory consists of the following main files and directories:

- `chat.py`: Contains the logic for handling chat operations and user queries.
- `embed.py`: Responsible for generating embeddings for the queries and responses.
- `main.py`: The entry point for starting the backend server.
- `scrape.py`: Handles web scraping operations.
- `requirements.txt`: Lists the Python dependencies required to run the backend.
- `.env`: Environment variables configuration (e.g., API keys, database URLs).
- `backend/`: Directory containing core backend functionality.

### Backend Requirements

Make sure to install the necessary Python packages by using the `requirements.txt` file:

```bash
pip install -r requirements.txt

Backend Setup Steps
Clone the repository:

bash
Copy
git clone <repository_url>
cd backend
Set up environment variables:

Create a .env file to store necessary configuration like API keys, database URLs, etc.

Install required dependencies:

bash
Copy
pip install -r requirements.txt
Run the backend server:

This is for common running command
bash
Copy
uvicorn main:app --host 0.0.0.0 --port 8000

Production
bash
uvicorn main:app --host 0.0.0.0 --port 8000 --workers 4
The backend should now be running and ready to process requests.

Backend Usage
Once the backend is running, it will provide functionality to handle various tasks like:

Chat Operations: Handle user queries and responses through chat interactions.

Embeddings: Generate embeddings from input text using pre-defined models.

Web Scraping: Fetch data from external sources using web scraping logic.

Frontend Setup
Frontend Project Structure
The frontend directory consists of the following main files and directories:

app/: Contains the main application code.

components/: Reusable UI components such as buttons, forms, and others.

public/: Static assets (e.g., images, icons).

styles/: CSS and styling-related files (e.g., TailwindCSS configurations).

next.config.ts: Configuration for the Next.js app.

package.json: Defines the dependencies and scripts for the frontend.

tailwind.config.ts: Configuration for TailwindCSS.

tsconfig.json: TypeScript configuration.

Frontend Requirements
Make sure to install the necessary Node.js packages by using the package.json file:

bash
Copy
npm install
Frontend Setup Steps
Clone the repository:

bash
Copy
git clone <repository_url>
cd frontend
Install dependencies:

bash
Copy
npm install
Run the frontend:

bash
Copy
npm run dev
This will start the Next.js development server on http://localhost:3000.

Frontend Usage
The frontend application communicates with the backend to perform the following tasks:

Render the User Interface: Displays components like forms, chat boxes, buttons, and other UI elements.

API Requests: Interacts with the backend API to send and receive data, such as user inputs and responses.

Display Data: Uses data fetched from the backend to update the frontend dynamically.

Project Workflow
Backend Workflow
User Input: The user sends a query or request through the frontend interface.

Backend Processing: The backend processes the request using the relevant functions, such as generating embeddings, fetching data via scraping, or handling chat interactions.

Response Generation: The backend generates a response and sends it back to the frontend.

Frontend Display: The frontend displays the response or result to the user, such as showing the processed chat or data.

Frontend Workflow
User Interaction: The user interacts with the UI components (e.g., typing a message in a chat box).

API Communication: The frontend sends a request to the backend via API calls.

Rendering the Data: The frontend receives the response from the backend and updates the UI accordingly.

Display Response: The user sees the updated information, such as chat replies or processed data.

License
This project is licensed under the MIT License - see the LICENSE file for details.


### Key Features:

1. **Backend:**
   - Handles core tasks like chat operations, embedding generation, and web scraping.
   - Allows communication via RESTful APIs to interact with the frontend.
   
2. **Frontend:**
   - Built using Next.js and TailwindCSS.
   - Displays dynamic UI components such as chatboxes and forms.
   - Interacts with the backend via API calls to fetch and display data.

3. **Usage:**
   - After setting up both backend and frontend, the system will allow users to interact with the RAG system, send queries, and view responses.

This README now covers both backend and frontend processes and provides a detailed flow of the project. Let me know if you need further modifications!
