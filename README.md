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

## 🚀 Installation

### Prerequisites
- Python 3.8+  
- pip  
- Git  

### Step 1: Clone Repository
```bash
git clone https://github.com/Shubhamraj1909/BottrainerNLUProject.git
cd BottrainerNLUProject

```
### Step 2: Create Virtual Environment

``
###### Windows
```bash
python -m venv venv
venv\Scripts\activate
```
###### Linux / Mac
```bash
python3 -m venv venv
source venv/bin/activate

```
### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```
### Step 4: Environment Variables

Create a .env file in the root directory:
```bash

# MySQL Database Configuration
DATABASE_URL=mysql+pymysql://username:password@localhost:3306/chatbot_nlu_db

# JWT Configuration
JWT_SECRET_KEY=your-secret-key
JWT_ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30

# File & Model Storage
MODEL_SAVE_PATH=./saved_models
UPLOAD_FOLDER=./uploaded_files

```
### Step 5: Initialize Database
```bash
# The database will be automatically created when you first run the backend
python newback.py
```
### Step 6: Run Application


###### Terminal 1 - Backend (FastAPI)
```bash

python newback.py
```
###### Terminal 2 - Frontend (Streamlit)
```bash
streamlit run newfront.py
```
 ###### Access URLs

Frontend: http://localhost:8501

Backend API: http://localhost:8000

API Documentation: http://localhost:8000/docs

### MySQL Database Setup
1. Install MySQL and create a database:
```bash
CREATE DATABASE chatbot_nlu_db;

2. Update .env with your MySQL credentials

3. Install MySQL connector:

```bash
pip install pymysql
```
### 📖 Usage

1. Register / Login

2. Create Workspace

3. Upload Dataset (CSV/JSON)

4. Annotate Data

5. Train Model

6. Evaluate Performance

7. Apply Active Learning
   

### 📁 Project Structure
```text
BottrainerNLUProject/
├── newback.py              # FastAPI Backend
├── newfront.py             # Streamlit Frontend
├── requirements.txt        # Python dependencies
├── runtime.txt             # Python version specification
├── traveldatasett.json     # Sample travel dataset
└── sportsdataset.json      # Sample sports dataset


```
### 🛠️ Tech Stack

| Component  | Technology           |
| ---------- | -------------------- |
| Frontend   | Streamlit            |
| Backend    | FastAPI              |
| Database   | mySql               |
| Auth       | JWT, bcrypt          |
| NLU        | spaCy, Rasa, BERT    |
| ML         | scikit-learn, pandas |
| Deployment | Docker               |

### 📅 Milestones

- Setup & Authentication ✅

- Annotation & Training ✅

- Evaluation & Reporting ✅

- Active Learning & Admin Panel ✅

### 📄 License

      MIT License.
  
 
### 🙏 Acknowledgments

- Open-source community

- Infosys Springboard Program

### 🔮 Future Enhancements

- Cloud deployment

- Multi-language support

- Real-time chatbot testing

- Advanced explainability







