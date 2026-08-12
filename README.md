# Hi there, I'm Nikhil 👋 
### **Data Engineer & Applied Machine Learning Architect**

I engineer production-grade machine learning pipelines, asynchronous web systems, and cloud data infrastructures. My work focuses on solving complex real-world challenges across **multimodal GenAI**, **clinical predictive modeling**, **enterprise ELT data architectures**, and **industrial IoT signal processing**.

---

## 🛠️ Core Tech Stack & Tooling

<div align="center">

  ### Languages & Core Runtimes
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![SQL](https://img.shields.io/badge/SQL-003B5C?style=for-the-badge&logo=sqlite&logoColor=white)
  ![Bash](https://img.shields.io/badge/GNU%20Bash-4EAA25?style=for-the-badge&logo=GNU%20Bash&logoColor=white)

  ### Machine Learning & Artificial Intelligence
  ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
  ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
  ![LightGBM](https://img.shields.io/badge/LightGBM-228B22?style=for-the-badge&logo=xgboost&logoColor=white)
  ![Google Gemini](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlecloud&logoColor=white)
  ![SHAP](https://img.shields.io/badge/SHAP-000000?style=for-the-badge&logo=python&logoColor=white)

  ### Data Engineering & Analytics Infrastructure
  ![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
  ![Microsoft SQL Server](https://img.shields.io/badge/SQL%20Server-CC292B?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
  ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
  ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)

  ### Serving, APIs & Vector Systems
  ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
  ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
  ![FAISS](https://img.shields.io/badge/FAISS%20Vector%20DB-008080?style=for-the-badge&logo=meta&logoColor=white)
  ![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white)

  ### Analytics & DevOps Tools
  ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)
  ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
  ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
  ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

---

## 🚀 Featured Portfolio Projects

### 1. 📻 AudiX Engine: Multimodal GenAI Ingestion & Semantic Discovery Pipeline
> **High-Throughput Asynchronous Audio Transcreation & Vector Search Framework**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Google Gemini](https://img.shields.io/badge/Google%20Gemini-8E75B2?style=flat-square&logo=googlecloud&logoColor=white)
![FAISS](https://img.shields.io/badge/FAISS-008080?style=flat-square&logo=meta&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)

* **Overview**: Built an enterprise-grade async transcreation and semantic content discovery engine for multi-lingual audio streaming networks.
* **Architecture & Innovation**:
  * **Asynchronous Orchestration**: Engineered a non-blocking FastAPI gateway using `asyncio.to_thread` and a dynamic `ThreadPoolExecutor(max_workers=4)` to decouple heavy network operations and audio synthesis from the ASGI event loop.
  * **Deterministic Hashing Cache**: Implemented SHA-256 cryptographic signature hashing on script inputs to achieve sub-millisecond cache hits and avoid redundant API costs.
  * **Fail-Safe OS Swaps**: Utilized isolated temporary files (`tempfile`) and atomic OS-level moves (`shutil.move`) to eliminate mid-write disk corruptions.
  * **Vector Discovery Engine**: Deployed `SentenceTransformers` mapped to a FAISS `IndexFlatIP` vector database, using $L_2$ normalization to convert fast inner product calculations into exact Cosine Similarity.
* 🔗 **[View Repository](https://github.com/itsnik101/AudiX-Engine)**

---

### 2. 🏥 PhysioNet ICU Mortality Prediction Framework
> **Hybrid Gradient Boosted & Deep Learning Clinical Decision Support System**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-228B22?style=flat-square&logo=xgboost&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

* **Overview**: Developed an end-to-end clinical machine learning framework to predict rare-event in-hospital mortality using sparse 48-hour irregular EHR time-series logs.
* **Architecture & Innovation**:
  * **Informative Missingness Masking**: Modeled clinical diagnostic omission as an explicit feature vector (`_is_missing = 1`), leveraging physician ordering intent as a key predictive signal.
  * **50/50 Hybrid Ensemble**: Combined LightGBM GBDT (for non-linear tabular threshold boundaries) with a PyTorch Bidirectional LSTM (for tracking 48-hour vital trajectory velocities).
  * **Platt Scaling Calibration**: Wrapped tree cross-validations inside an out-of-fold `CalibratedClassifierCV` layer to map raw model outputs to true empirical clinical probabilities.
  * **Native Explainability**: Integrated consensus TreeSHAP attributions and mapped clean medical terminology (`CLINICAL_VOCABULARY`) upstream at feature construction.
* 🔗 **[View Repository](https://github.com/itsnik101/ICU-Mortality-Prediction)**

---

### 3. 💳 Credit Risk Analytics & Engineering Pipeline
> **Automated ELT Data Pipeline, Anomaly Auditing & Risk Intelligence System**

![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC292B?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

* **Overview**: Refactored static credit risk SQL analysis into an automated, modular ELT data pipeline servicing interactive BI dashboards.
* **Architecture & Innovation**:
  * **Python Data Ingestion**: Built a programmatic loading engine via `SQLAlchemy` to ingest raw loan applications directly into SQL Server landing tables.
  * **Modular dbt Modeling**: Created layered staging (`stg_loans`) and marts models (`fct_risk_analytics`, `fct_income_quartiles`) to eliminate redundant queries and build a single source of truth.
  * **Risk Anomaly Auditing**: Engineered custom validation models (`fct_risk_anomalies`) to automatically flag high-credit rejections (>700 score) and low-credit approvals (<600 score).
  * **Executive BI Dashboard**: Designed a high-density interactive Tableau Public dashboard featuring dynamic parameters, action filters, and demographic exposure matrices.
* 🔗 **[View Repository](https://github.com/itsnik101/credit-risk-analytics-pipeline)**

---


## 📬 Connect With Me

* 💼 **LinkedIn**: https://www.linkedin.com/in/nikhil-rawat-1b5059250/
* 📧 **Email**: nikhilr0876@gmai.com
