# Project README

## 💻 Tech Stack

### Backend
- **Framework:** Flask
- **Database:** SQLite (via SQLAlchemy ORM)
- **AI:** Grok API (model: `llama-3.3-70b-versatile` for item extraction)
- **Libraries:** `flask-cors`, `python-dotenv`, `datetime`

### Frontend
- **Framework:** React (TypeScript)
- **Styling:** Tailwind CSS
- **API Client:** Axios
- **Chat History:** Stored in `localStorage`

---

## 🛠️ Installation and Setup

### 1. Prerequisites
- Python 3.x
- Node.js and npm/yarn
- Grok API Key

---

## 2. Backend Setup (`server/`)

### Step 1: Clone and Navigate
Clone the repository and move into the backend directory.

### Step 2: Create Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source .venv/Scripts/Activate.ps1
```

### Step 3: Install Python Dependencies
```bash
pip install -r requirements.txt
```
The requirements should include:
- Flask
- Flask-CORS
- SQLAlchemy
- python-dotenv
- groq
- requests

### Step 4: Add Environment Variables
Create a `.env` file inside the backend folder:
```env
GEMINI_API_KEY="ADD_YOUR_API_KEY_HERE"
```

### Step 5: Initialise the Database
```bash
python db_init.py
```
You should see a confirmation message such as:
```
Database Ready
```

### Step 6: Start the Flask Server
```bash
python app.py
```
The server will run at:
```
http://127.0.0.1:8000
```

---

## 3. Frontend Setup (`client/`)

### Step 1: Navigate to Client Directory
```bash
cd client
```

### Step 2: Install Node Dependencies
```bash
npm run install
```

### Step 3: Start the Development Server
```bash
npm run start
```

Your app will be live at:
```
http://localhost:5173
```

---

## 🚀 Overview
This project delivers a full-stack application integrating a React + TypeScript frontend with a Flask backend and the Google Gemini AI model. It supports item extraction, persistent chat history, and a clean developer workflow.

---

## 📂 Project Structure
```
root/
├── server/
│   ├── app.py
│   ├── db_init.py
│   ├── models.py
│   ├── requirements.txt
│   ├── .env
│   └── ...
└── client/
    ├── src/
    │  ├─── App.tsx
    │  ├─── components/
    │  │    ├─── ChatBox.tsx
    │  │    ├─── GroceryList.tsx 
    │  ├─── utils
    │  │    ├─── AxiosInstance.ts 
    │  ├─── ...      
    ├── package.json
    └── ...
```

---
---

