# **AI-Powered Finance Management Tool**  

This project leverages cutting-edge technologies like **Django Rest Framework**, **Next.js**, and **OpenAI's GPT-3.5** to transform how users **track income, manage expenses, and gain AI-driven financial insights**. With an intuitive interface and intelligent automation, this tool simplifies **financial decision-making** and empowers users to optimize their budget effectively.  

---

## **🌟 Features at a Glance**  

### 📊 **Track Your Finances**  
- Log **income and expenses** with categories, amounts, and dates.  
- Maintain a **detailed record** of financial transactions for easy tracking.  

### 📈 **Generate Reports**  
- View **monthly and yearly summaries** of financial activity.  
- Identify **spending patterns and areas for improvement** with visual analytics.  

### 🤖 **AI-Powered Assistance**  
- Get **personalized budgeting tips** based on spending behavior.  
- Use an **intelligent chatbot (powered by OpenAI's GPT-3.5)** to get answers to financial queries and planning advice.  

---

## **💻 Tech Stack Highlights**  

| **Component**   | **Technology** |
|---------------|----------------|
| **Backend**   | Django Rest Framework (DRF) |
| **Frontend**  | Next.js (React-based UI) |
| **Database**  | PostgreSQL |
| **AI Integration**  | OpenAI's GPT-3.5 |
| **Authentication**  | JWT-based authentication |
| **Deployment**  | Docker, AWS/GCP |

---

## **🚀 Getting Started**  

### **1️⃣ Installation**  
Ensure you have **Python 3.8+**, **Node.js**, and **Docker** installed. Then, clone the repository:  

```bash
git clone https://github.com/your-repo/finance-ai.git
cd finance-ai
```

---

### **2️⃣ Backend Setup (Django Rest Framework)**  
Navigate to the `backend/` directory and install dependencies:  

```bash
cd backend
pip install -r requirements.txt
```

Run database migrations:  

```bash
python manage.py migrate
```

Start the backend server:  

```bash
python manage.py runserver
```

---

### **3️⃣ Frontend Setup (Next.js)**  
Navigate to the `frontend/` directory and install dependencies:  

```bash
cd ../frontend
npm install
```

Run the Next.js development server:  

```bash
npm run dev
```

---

### **4️⃣ Environment Variables Configuration**  
Create a `.env` file in both the `backend/` and `frontend/` directories and configure:  

#### **Backend (`backend/.env`):**  
```
OPENAI_API_KEY=your_openai_api_key
DATABASE_URL=your_database_connection_string
SECRET_KEY=your_django_secret_key
```

#### **Frontend (`frontend/.env`):**  
```
NEXT_PUBLIC_BACKEND_URL=http://localhost:8000
OPENAI_API_KEY=your_openai_api_key
```

---

## **🛠 API Endpoints**  

| **Endpoint**  | **Method** | **Description** |
|--------------|-----------|----------------|
| `/api/transactions/` | `GET` | Fetch all transactions |
| `/api/transactions/` | `POST` | Add a new transaction |
| `/api/reports/monthly/` | `GET` | Get monthly financial summary |
| `/api/reports/yearly/` | `GET` | Get yearly financial summary |
| `/api/ai/chat/` | `POST` | AI chatbot financial advice |

Example request to fetch transactions:
```bash
curl -X GET http://localhost:8000/api/transactions/
```

---

## **🚀 AI-Powered Chatbot Usage**  
- Users can input financial questions like:  
  **"How much did I spend last month on groceries?"**  
  **"Suggest a budget plan for saving $500 per month."**  
- The chatbot, powered by **OpenAI's GPT-3.5**, provides real-time financial insights.

---

## **📊 Future Enhancements**  
✅ Integrate **real-time currency conversion**.  
✅ Implement **automatic categorization** of transactions using AI.  
✅ Add **predictive analytics** for financial forecasting.  
✅ Deploy on **AWS/GCP** with scalable microservices.  

---

