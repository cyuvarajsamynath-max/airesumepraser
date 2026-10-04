# AI Resume Parser

A full-stack application that extracts text from a resume PDF, uses a Large Language Model (Google Gemini) to parse it into structured data, provides a score and specific suggestions for improvement, and matches the resume against a job description.

## Project Structure
- `backend/`: Python 3.11+ FastAPI server handling PDF extraction, AI parsing, and scoring.
- `frontend/`: React application (built with Vite) for the user interface.

## Prerequisites
- Node.js (v18+)
- Python (3.11+)
- A [Google Gemini API Key](https://aistudio.google.com/app/apikey)

## Phase 1: Setup Instructions

### Backend Setup
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Create and activate a Python virtual environment:
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Mac/Linux:
   source venv/bin/activate
   ```
3. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file by copying `.env.example` and add your Gemini API Key:
   ```bash
   cp .env.example .env
   ```
5. Run the development server:
   ```bash
   uvicorn main:app --reload
   ```
   The backend will be running at `http://127.0.0.1:8000`. You can check the health route at `http://127.0.0.1:8000/health`.

### Frontend Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install the npm dependencies:
   ```bash
   npm install
   ```
3. Start the Vite development server:
   ```bash
   npm run dev
   ```
   The frontend will be running at `http://localhost:5173`.
