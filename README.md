<h1 align="center">Hi, I'm Youssef 👋</h1>
<p align="center">
  <em>Data Engineer</em><br>
  🎓 B.Sc. in <strong>Computer Engineering, Suez Canal University</strong><br>
  🏛️ <strong>Information Technology Institute (ITI)</strong> — Data Engineering Program<br>
  <sub>End-to-end data engineering · SQL · dbt · ETL/ELT · Data Warehousing · Spark · Kafka · Airflow</sub>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/SQL-%2300758F.svg?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/PySpark-%23E25A1C.svg?style=for-the-badge&logo=apache-spark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Data%20Warehousing-%230072C6.svg?style=for-the-badge&logo=amazondynamodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kafka-%23231F20.svg?style=for-the-badge&logo=apache-kafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-%23017CEE.svg?style=for-the-badge&logo=apache-airflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/dbt-%23FF694B.svg?style=for-the-badge&logo=dbt&logoColor=white"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/youssef-m-makram"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:youssef.m.makram.m@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://wa.me/201039155852"><img src="https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="WhatsApp"></a>
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YoussefMakram27&show_icons=true&theme=tokyonight" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YoussefMakram27&layout=compact&theme=tokyonight" height="165"/>
</p>

---

## 🚀 About Me

- 🎓 B.Sc. in Computer Engineering, Suez Canal University
- 🏛️ Graduated from the Information Technology Institute (ITI) Data Engineering program
- 🏥 Capstone: Raqib, a healthcare data platform with a Kafka + Spark streaming layer and an Airflow + S3 + Snowflake + dbt batch layer
- 🧠 Skilled in **SQL**, **Python**, and **PySpark**, with hands-on experience in **Kafka** and growing expertise in **Airflow** and **dbt**.


---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Languages** | Python, SQL (T-SQL) |
| **Batch & Orchestration** | PySpark, Pandas, Apache Airflow |
| **Streaming** | Apache Kafka (KRaft, Schema Registry, Connect), Spark Structured Streaming |
| **Warehouse & Lake** | Snowflake, AWS S3, SQL Server, PostgreSQL, Parquet |
| **Transformation & Quality** | dbt, Great Expectations |
| **Modeling** | Medallion architecture, star schema, galaxy schema |
| **Visualization** | Power BI |
| **Version Control** | Git, GitHub |

---

## 📌 Featured Projects

### 🏥 [Raqib: Healthcare Data Intelligence Platform](https://github.com/YoussefMakram27/Raqib-Healthcare-Data-Intelligence-Platform)
**ITI graduation project, built with a team of five**
 
A healthcare platform that unifies clinical workflows with two pipelines: a real-time layer and a batch warehouse layer.
 
```
Real-time:  Receptionist → Kafka (3 brokers) → Doctor / Lab consumers → Spark Streaming → PostgreSQL
Batch:      PostgreSQL → Airflow → S3 (Parquet) → Snowflake → dbt (staging → intermediate → marts)
Serving:    Power BI dashboard · RAG chatbot (Ollama) · Grafana + Prometheus monitoring
```
 
- **Fault-tolerant streaming:** 3-broker KRaft Kafka cluster, replication factor 3, `acks=all` and idempotent producers
- **Warehouse:** dbt models for 11 staging, 4 intermediate, 9 dimension and 7 fact tables (galaxy schema), with automated dbt tests
- **Orchestration:** daily Airflow DAGs for Postgres → S3 → Snowflake and for `dbt run` + `dbt test`
- **Serving:** 6-page Power BI report over ~5.6M encounters, plus a Streamlit RAG chatbot that answers questions about patient records
- **Observability:** Kafka consumer lag and Postgres metrics in Grafana, auto-provisioned
- **Infra:** 17+ services in one Docker Compose file
**Stack:** Kafka · PySpark · Airflow · S3 · Snowflake · dbt · Docker · Grafana · Power BI · Ollama
 
---
 
### 🚕 [Uber Real-Time Trip Analytics Pipeline](https://github.com/YoussefMakram27/Uber-Real-Time-Analytics-Pipeline)
 
Streams NYC taxi trips through Kafka, then processes and enriches them with Spark and stores the results in SQL Server and Parquet.
 
```
Parquet → Kafka Producer → Topic: uber_trips
                              ├─→ SQL Server Consumer
                              └─→ Spark Structured Streaming → Raw Parquet
                                                                  └─→ Spark Batch Cleaner → Cleaned Parquet
```
 
- Producer resumes after a restart and only saves its state once Kafka confirms delivery
- Cleaning step: dedupe, fix swapped timestamps, validate distance, fare and speed
- Derived features: `trip_duration_minutes`, `avg_speed_mph`, `is_high_quality`
**Stack:** Python · Kafka · Spark Structured Streaming · PySpark · SQL Server · Parquet
 
---
 
### 🏭 [ERP–CRM Integration for Supply Chain Optimization](https://github.com/YoussefMakram27/ERP-CRM-Integration-for-Supply-Chain-Optimization)
 
Combines siloed ERP (inventory, suppliers, purchasing) and CRM (sales, customers, returns) data into one warehouse for supply chain analytics.
 
- **Bronze → Silver → Gold** layers, with MERGE (upsert) logic for incremental loads
- Star schema with **4 fact tables** and **5 dimensions**
- Enables sales performance, low-stock detection, return analysis and supplier evaluation
**Stack:** SQL · Medallion Architecture · Dimensional Modeling

---
<p align="center"> 💬 Open to <b>data engineering</b> roles. Feel free to reach out! </p>
