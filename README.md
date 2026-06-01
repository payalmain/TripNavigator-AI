# ✈️ TripNavigator AI

## AI-Powered Multi-Agent Travel Planning System using LangGraph

TripNavigator AI is a real-world Multi-Agent AI application built using LangGraph. The system orchestrates multiple specialized AI agents to automatically plan complete travel experiences, including flight discovery, hotel recommendations, itinerary generation, and final trip planning.

---

## 🚀 Features

* ✈️ Flight Search Agent
* 🏨 Hotel Recommendation Agent
* 🗓️ Itinerary Planning Agent
* 🤖 Final Response Agent
* 🧠 Persistent Memory using PostgreSQL
* 🌐 Real-Time API Integration
* 💻 Interactive Streamlit Web Interface
* 🔄 Multi-Agent Workflow Orchestration with LangGraph

---

## 🏗️ Architecture

The system consists of four AI agents:

1. **Flight Agent**

   * Searches available flight information.

2. **Hotel Agent**

   * Finds hotel recommendations based on destination and travel preferences.

3. **Itinerary Agent**

   * Creates a complete day-by-day travel itinerary.

4. **Final Agent**

   * Combines flight, hotel, and itinerary information into a final travel plan.

---

## 🛠️ Tech Stack

* Python
* LangGraph
* LangChain
* Groq
* Llama 3.3 70B
* PostgreSQL
* Streamlit
* Tavily Search API
* AviationStack API

---

## 📂 Project Structure

```text
TripNavigator-AI/
│
├── frontend.py
├── main.py
├── requirements.txt
├── .env
├── tool/
│   ├── flight_tool.py
│   └── tavily_tool.py
│
└── travel_plans/
```

---

## ⚙️ Setup Instructions

### Step 1: Create Virtual Environment

```bash
python -m venv langgraph_env3
```

### Activate Environment

**Windows**

```bash
langgraph_env3\Scripts\activate
```

---

 ### Step 2: Install Dependencies

Install all required packages using the requirements file:

```bash
pip install -r requirements.txt
```


### Step 3: Install PostgreSQL

Download PostgreSQL:

https://www.postgresql.org/download/

During installation remember:

* PostgreSQL Username
* PostgreSQL Password
* Port Number

---

### Step 4: Create Database

```sql
CREATE DATABASE DATABASE_NAME;
```

---

### Step 5: Configure Environment Variables

Create a `.env` file inside the project root.

```env
GROQ_API_KEY=***********************

TAVILY_API_KEY=***********************

AVIATIONSTACK_API_KEY=***********************

DATABASE_URL=postgresql:***********************
```

---

## 🔑 API Keys

### Groq

https://console.groq.com

### Tavily

https://tavily.com

### AviationStack

https://aviationstack.com

---

## ▶️ Running the Application

### Run in Terminal

```bash
python main.py
```

---

### Run Streamlit UI

```bash
streamlit run frontend.py
```

---

## 🧪 Example Prompt

```text
Plan a complete 7-day Japan trip including flights, hotels, and sightseeing under ₹2 lakhs.
```

---

## 🔄 Workflow

```text
User Query
    │
    ▼
Flight Agent
    │
    ▼
Hotel Agent
    │
    ▼
Itinerary Agent
    │
    ▼
Final Agent
    │
    ▼
Travel Plan Generated
    │
    ▼
Stored in PostgreSQL Memory
```

---

## 🎯 Key Highlights

* Multi-Agent AI System
* Persistent Conversation Memory
* Real-Time Travel Planning
* LangGraph Workflow Orchestration
* Production-Ready Architecture
* Interactive Streamlit Interface

---
