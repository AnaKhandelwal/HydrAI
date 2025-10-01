**HydrAI**

💧 AI-Powered Groundwater Insights Platform

An AI-powered system delivering **real-time groundwater insights** across **733 districts** in India using **CGWB and state datasets**.  

The platform combines:
- 🧠 **AI chatbot** for natural-language queries  
- 📊 **Interactive dashboards** with district-level visualizations  
- 🔮 **Predictive modeling** for groundwater stress analysis  

Built to make groundwater intelligence accessible to **farmers, NGOs, and policymakers**.

---

## 🚀 Features

- **Chatbot Interface**
  - Natural language queries
  - LLM-powered retrieval with contextual answers
  - User vs. bot styled chat bubbles

- **Visualization Sidebar**
  - Groundwater status distribution
  - Trend analysis (2017–2024)
  - State-wise tabular insights
  - Tabs: *Charts | Maps | Data*

- **Predictive Modeling**
  - Derived features: stress indices, recharge efficiency, seasonal trends
  - Achieves >80% accuracy in stress prediction

- **Deployment**
  - Working prototype combining **FastAPI backend** + **React frontend**
  - Deployed with **ngrok** (prototype-ready for cloud)

---

## 📊 Tech Stack

- **Frontend:** ReactJS  
- **Backend:** FastAPI  
- **LLM/RAG:** LangChain + LlamaIndex  
- **Database:** Supabase  
- **Visualization:** Plotly / Matplotlib  
- **Deployment:** ngrok / cloud-ready  

---

## 📂 Project Structure
project/
│── backend/ # FastAPI app + LLM pipeline
│ ├── app.py # API routes
│ ├── models/ # ML + LLM models
│ └── db/ # Supabase integration
│
│── frontend/ # HTML/CSS/JS app
│ ├── index.html # Landing page + sidebar
│ ├── chatbot.html # Chat interface
│ ├── style.css # Styling for UI
│ └── script.js # Handles chat + API calls
│
│── datasets/ # Groundwater datasets (CGWB + state)
│── README.md # Documentation

---

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/your-username/groundwater-ai.git
cd groundwater-ai
```
#Backend (FastAPI)
```bash
Copy code
cd backend
pip install -r requirements.txt
uvicorn app:app --reload
```
#Frontend (HTML)
Open frontend/index.html in your browser

Or serve it locally:

```bash
Copy code
cd frontend
python -m http.server 8001
```
Access at: http://localhost:8001
Access the app
Frontend: http://localhost:8001 (or open HTML directly)

Backend API: http://localhost:8000

