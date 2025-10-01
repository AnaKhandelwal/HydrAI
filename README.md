# HydrAI
💧 AI-Powered Groundwater Insights Platform

This project is an AI-powered system that delivers real-time groundwater insights across 733 districts in India, using CGWB and state datasets.

It combines an AI chatbot interface for natural-language queries with interactive dashboards for district-level visualization, making groundwater intelligence accessible to farmers, NGOs, and policymakers.

🚀 Features

AI Chatbot Interface

Ask questions in natural language about groundwater conditions.

LLM-powered retrieval with context-aware responses.

Integrated into a clean chat UI with user vs. bot message styling.

Visualization Sidebar

District-level charts and stats.

Trend analysis (2017–2024).

Tabbed dashboards: Charts | Maps | Data.

Predictive Modeling

Derived features (stress indices, recharge efficiency, seasonal trends).

80% accuracy in groundwater stress prediction.

Deployment

Fully working prototype deployed with FastAPI backend + React frontend.

📊 Tech Stack

Data Layer: Supabase

AI/LLM: LangChain
 + LlamaIndex

Backend: FastAPI

Frontend: ReactJS (chat + visualization dashboard)

Visualization: Plotly / Matplotlib

Hosting: ngrok (prototype) / cloud deployment-ready

📂 Project Structure
project/
│── backend/              # FastAPI app + LLM pipeline
│   ├── app.py            # FastAPI routes
│   ├── models/           # ML + LLM models
│   └── db/               # Supabase integration
│
│── frontend/             # React app (chat + sidebar)
│   ├── src/
│   │   ├── components/   # Chat UI, Sidebar, Tabs
│   │   ├── App.js
│   │   └── index.js
│   └── public/
│
│── datasets/             # Groundwater datasets (CGWB + state)
│── README.md             # Documentation

⚙️ Installation & Setup

Clone this repository

git clone https://github.com/your-username/groundwater-ai.git
cd groundwater-ai


Backend (FastAPI)

cd backend
pip install -r requirements.txt
uvicorn app:app --reload


Frontend (React)

cd frontend
npm install
npm start


Access the system

Frontend (Chat + Dashboard) → http://localhost:3000

Backend (API/LLM) → http://localhost:8000

🎯 Use Cases

Farmers: Get district-level insights for irrigation planning.

NGOs: Monitor groundwater stress for sustainable projects.

Policymakers: Access real-time analytics for water resource management.
