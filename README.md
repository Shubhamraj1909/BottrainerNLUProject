# 🤖 Chatbot NLU Trainer & Evaluator

An end-to-end platform for building, training, evaluating, and improving Natural Language Understanding (NLU) models for enterprise chatbots.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat&logo=fastapi)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📋 Table of Contents
- Overview  
- Features  
- Architecture  
- Installation  
- Usage  
- Project Structure  
- Tech Stack  
- Milestones  
- Contributing  
- License  
- Team  

---

## 🌟 Overview
The **Chatbot NLU Trainer & Evaluator** is a comprehensive platform designed to streamline the development of intelligent chatbots. It provides an integrated solution for dataset management, annotation, model training, evaluation, and continuous improvement using active learning.

**Key Problem Solved:**  
Traditional chatbot development relies on separate tools for annotation, training, and evaluation. This platform unifies the entire workflow, making chatbot development faster, more efficient, and accessible to both technical and non-technical users.

---

## ✨ Features

### 🔐 Security & Access Control
- JWT-based authentication with bcrypt password hashing  
- Role-based access control (Admin/User)  
- Secure workspace isolation  
- Session management  

### 📊 Dataset Management
- Upload datasets in CSV/JSON formats  
- Visualize intent and entity distribution  
- Dataset versioning and tracking  
- Configurable train/test split  

### 🏷️ Annotation Interface
- Interactive intent tagging  
- Visual entity span highlighting  
- Batch annotation support  
- Export annotated datasets  

### 🤖 Model Training
- Supports multiple NLU frameworks:
  - **spaCy** – Fast, production-ready models  
  - **Rasa** – Conversational AI framework  
  - **BERT** – Transformer-based models  
- Hyperparameter configuration  
- Model versioning  
- Background training with progress tracking  

### 📈 Evaluation & Analytics
- Metrics: Accuracy, Precision, Recall, F1-Score  
- Confusion matrix visualization  
- Confidence score analysis  
- Model comparison across versions  
- Exportable reports  

### 🔄 Active Learning
- Identify low-confidence predictions  
- Smart sampling for manual review  
- Continuous improvement loop  
- Reduces annotation effort by 40–60%  

### 👨‍💼 Admin Dashboard
- User management  
- Workspace monitoring  
- System analytics  
- Model deployment management  

---

## 🏗️ Architecture
┌─────────────────────────────────────────────────────────────┐
│ Streamlit Frontend │
│ (Auth • Dashboard • Annotation • Evaluation) │
└──────────────────────────────┬──────────────────────────────┘
│
┌──────────────────────────────▼──────────────────────────────┐
│ FastAPI Backend │
│ (REST API • Business Logic • Model Orchestration) │
└──────────────────────────────┬──────────────────────────────┘
│
┌──────────────────────────────▼──────────────────────────────┐
│ SQLite Database │
│ (Users • Workspaces • Datasets • Models • Feedback) │
└──────────────────────────────┬──────────────────────────────┘
│
┌──────────────────────────────▼──────────────────────────────┐
│ NLU Model Ecosystem │
│ (spaCy • Rasa • BERT • Custom Models) │
└─────────────────────────────────────────────────────────────┘

yaml
Copy code

---

## 🚀 Installation

### Prerequisites
- Python 3.8+  
- pip  
- Git  

### Step 1: Clone Repository
```bash
git clone https://github.com/yourusername/chatbot-nlu-platform.git
cd chatbot-nlu-platform
Step 2: Create Virtual Environment

```bash
# Windows
python -m venv venv
venv\Scripts\activate

```bash
# Linux / Mac
python3 -m venv venv
source venv/bin/activate
Step 3: Install Dependencies

```bash
pip install -r requirements.txt
Step 4: Environment Variables
Create a .env file:

env
Copy code
DATABASE_URL=sqlite:///./chatbot_nlu.db
JWT_SECRET_KEY=your-secret-key
JWT_ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30
MODEL_SAVE_PATH=./saved_models
UPLOAD_FOLDER=./uploaded_files
Step 5: Initialize Database
bash
Copy code
python backend/init_db.py
Step 6: Run Application
bash
Copy code
# Backend
cd backend
uvicorn app.main:app --reload --port 8000

# Frontend
cd frontend
streamlit run Home.py
Access URLs

Frontend: http://localhost:8501

Backend API: http://localhost:8000

Swagger Docs: http://localhost:8000/docs

📖 Usage
Register/Login

Create Workspace

Upload Dataset (CSV/JSON)

Annotate Data

Train Model

Evaluate Performance

Apply Active Learning

📁 Project Structure
kotlin
Copy code
chatbot-nlu-platform/
├── backend/
├── frontend/
├── data/
├── saved_models/
├── uploaded_files/
├── docs/
├── docker-compose.yml
├── requirements.txt
└── README.md
🛠️ Tech Stack
Component	Technology
Frontend	Streamlit
Backend	FastAPI
Database	SQLite
Auth	JWT, bcrypt
NLU	spaCy, Rasa, BERT
ML	scikit-learn, pandas
Deployment	Docker

📅 Milestones
Setup & Auth ✅

Annotation & Training ✅

Evaluation & Reporting ✅

Active Learning & Admin Panel ✅

🤝 Contributing
bash
Copy code
git checkout -b feature/YourFeature
git commit -m "Add new feature"
git push origin feature/YourFeature
Open a Pull Request 🚀

📄 License
Licensed under the MIT License.

👥 Team
Shubham Raj – Project Lead & Developer

Team Members – Contributors

Guide: Naveena – Project Mentor

🙏 Acknowledgments
Open-source community

Infosys Springboard Program

🔮 Future Enhancements
Cloud deployment

Multi-language support

Real-time chatbot testing

Advanced explainability

📞 Support
Use GitHub Issues

Email: your.email@example.com

yaml
Copy code

---

If you want, I can:
- Optimize this for **recruiters**
- Add **screenshots section**
- Shorten it for **hackathons**
- Create a **portfolio-friendly version**

Just tell me 👍






