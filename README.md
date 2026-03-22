<h1 align="center">Hi, I'm Youssef 👋</h1>
<p align="center">
  <em>Data Engineer & Analyst</em><br>
  🎓 B.Sc. in <strong>Computer Engineering, Suez Canal University</strong><br>
  🏛️ <strong>Information Technology Institute (ITI)</strong> — Data Engineering Program <em>(Jan 2026 – Present)</em><br>
  <sub>End-to-end data engineering · ETL/ELT · Data Warehousing · Stream Processing · Spark · Kafka · Airflow</sub>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-%233776AB.svg?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-%2300758F.svg?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/PySpark-%23E25A1C.svg?style=for-the-badge&logo=apache-spark&logoColor=white"/>
  <img src="https://img.shields.io/badge/Data%20Warehousing-%230072C6.svg?style=for-the-badge&logo=amazondynamodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/Kafka-%23231F20.svg?style=for-the-badge&logo=apache-kafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/Airflow-%23017CEE.svg?style=for-the-badge&logo=apache-airflow&logoColor=white"/>
  <img src="https://img.shields.io/badge/dbt-%23FF694B.svg?style=for-the-badge&logo=dbt&logoColor=white"/>
</p>

<p align="center">
  📧 <a href="mailto:youssef.m.makram.m@gmail.com">Email</a> •
  💼 <a href="https://www.linkedin.com/in/youssef-m-makram-m-osman-659a56233/" target="_blank">LinkedIn</a> •
  💻 <a href="https://github.com/YoussefMakram27" target="_blank">GitHub</a> •
  📱 <a href="https://wa.me/201281446248" target="_blank">WhatsApp</a>
</p>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YoussefMakram27&show_icons=true&theme=tokyonight" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YoussefMakram27&layout=compact&theme=tokyonight" height="165"/>
</p>

---

## 🚀 About Me

- 🧩 Passionate about designing and building scalable **data pipelines** — from raw ingestion to clean, analytics-ready data.
- 🧠 Skilled in **SQL**, **Python**, and **PySpark**, with hands-on experience in **Kafka** and growing expertise in **Airflow** and **dbt**.
- 🔁 I've built real-time streaming pipelines end-to-end: Kafka → Spark Structured Streaming → SQL Server / Parquet.
- 🎯 Goal: Become a full-stack **Data Engineer** capable of designing, automating, and optimizing end-to-end pipelines at scale.
- 🌱 Learning next: **Airflow → dbt → cloud-native stacks (AWS/GCP)**.

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| **Languages** | Python, SQL |
| **Data Processing** | PySpark, Pandas, Spark Structured Streaming |
| **Streaming** | Apache Kafka (confluent-kafka) |
| **Storage** | SQL Server, Parquet (Snappy) |
| **Orchestration** | Airflow *(learning)* |
| **Transformation** | dbt *(learning)* |
| **Visualization** | Power BI |
| **Version Control** | Git, GitHub |

---

## 📌 Featured Projects

### 🚕 [Uber Real-Time Trip Analytics Pipeline](https://github.com/YoussefMakram27/uber-realtime-pipeline)

> End-to-end real-time pipeline streaming NYC taxi trips through Kafka, processing with Spark, and persisting to SQL Server and Parquet.

**Tech:** Python · Apache Kafka · Spark Structured Streaming · PySpark · SQL Server · Parquet
```
Parquet File → Kafka Producer → Kafka Topic (uber_trips)
                                       │
                    ┌──────────────────┴──────────────────┐
                    ▼                                      ▼
           SQL Server Consumer               Spark Structured Streaming
           (confluent-kafka)                  → Raw Parquet sink
                                                      │
                                                      ▼
                                             Spark Batch Cleaner
                                              → Cleaned Parquet
```

**Highlights:**
- Stateful producer with resume-on-restart via `producer_state.json`
- Kafka delivery confirmation before saving offset state
- Spark cleaning: deduplication, timestamp correction, speed/distance/fare validation
- Derived features: `trip_duration_minutes`, `avg_speed_mph`, `is_high_quality`

---

### 🏭 [ERP–CRM Integration for Supply Chain Optimization](https://github.com/YoussefMakram27/ERP-CRM-Integration-for-Supply-Chain-Optimization)

> Integrates ERP (inventory & suppliers) and CRM (sales & customers) into a unified data warehouse for supply chain insights.

**Tech:** SQL · Medallion Architecture (Bronze → Silver → Gold)

**Highlights:**
- Star schema: 4 Fact tables + 5 Dimension tables
- Data cleaning, validation, and incremental loading
- Scalable and automation-ready design

---

## 📈 What I'm Working Toward
```
Current:   Kafka ✅ | Spark Streaming ✅ | SQL Warehousing ✅
Next:      Airflow (orchestration) → dbt (transformation) → Cloud (AWS/GCP)
Goal:      End-to-end automated, cloud-native data platform
```
