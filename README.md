# OJI AI-augmented NLP Project Management System 

The **OJI Project Management System** is a web-based application developed in **Python (Django)** that leverages **Natural Language Processing (NLP)** to enhance project management processes. It provides a centralized platform for project managers and team members to track project progress, manage resources, and collaborate effectively.  

The system is built on a robust and scalable architecture that integrates:  
- A traditional **relational database** for structured project data  
- A modern **vector database** for AI-powered features such as semantic search  

This hybrid approach ensures reliability in handling structured data, while also leveraging NLP and vector embeddings for intelligent data retrieval and analysis.

---

### Features
- End-to-end project flow management (Vision → Outcomes → Deliverables → Tasks)  
- AI-assisted semantic search across project artefacts (NLP-powered)  
- Cascade updates when editing project flows  
- Task assignment and progress tracking  
- Centralized collaboration platform  
- Hybrid relational + vector data storage  
- Evaluation scripts for data integration and scalability testing  

---

### Technologies
- **Python 3.10+**  
- **Natural Language Processing (NLP)** with OpenAI API  
- Django (web framework)  
- Relational Database (SQLite/PostgreSQL)  
- Vector Database (Chroma)  
- HTML, CSS, JavaScript (frontend)  

---

### User Guide

#### 1. Clone the Repository
git clone https://github.com/your-username/your-repo-name.git  
cd your-repo-name  

Check Python version (must be 3.10 or higher):  
python --version  

#### 2. Create and Activate Virtual Environment
Mac/Linux:  
python -m venv venv  
source venv/bin/activate  

Windows:  
python -m venv venv  
venv\Scripts\activate  

#### 3. Install Dependencies
pip install -r requirements.txt  

#### 4. Get an OpenAI API Key
1. Sign in or create an account at https://platform.openai.com/account/api-keys  
2. Click **Create new secret key** and copy it  
3. Create a `.env` file in the project root (`pm_app`) and add:  
   OPENAI_API_KEY="your-api-key-here"  
   USE_MOCK="FALSE"  
   EVAL_MODEL="gpt-4o"  

#### 5. Run the Application
python manage.py runserver  

This will start a local development server at:  
http://127.0.0.1:8000/  

Copy and paste the link into your browser to begin planning projects.

---

### Developer Guide

#### Run LLM Benchmarking
python llm_benchmark.py  

This will create a `benchmarks` folder in the project directory.

#### Run Evaluation Scripts
For evaluation functions in the pm_eval folder (`data_integration_eval.py` and `scalability_test.py`), insert your API key at the top of each file before execution.

---

### Authors
Developed collaboratively by the **QMUL MSc Business Data Analytics Student Team** as part of the *BUSM130 Capstone Project in Business Analytics* module.  
