# GenBI-Agent (v1)
*A Generative Business Intelligence Agent for enterprise analytics*  

---

## Overview  
GenBI Agent v1 is a **production-style AI analytics agent** built during the Chubb Hackathon. It transforms **natural language queries into SQL**, executes them on **Snowflake**, and returns **tables, dashboards, and narrative insights**.  

Unlike traditional BI dashboards, GenBI works as an **end-to-end analytics copilot**:  
- Understands domain-specific queries (insurance-focused in v1).  
- Generates SQL dynamically with schema awareness and retry loops.  
- Produces **interactive dashboards** and **automated anomaly detection**.  
- Provides **narrative business insights**, not just charts.  

---

## Tech Stack  
- **Frontend:** Streamlit  
- **Backend:** Python (NL-SQL pipeline, retry engine)  
- **LLM:** GPT-4 (via ChubbGPT API wrapper)  
- **Database:** Snowflake (private key auth)  
- **Visualization:** Plotly (via visualization agent)  

---

## Features in v1  
- Natural language → SQL (Snowflake dialect aware)  
- Schema-grounded query generation (via JSON schema descriptions)  
- Domain-aware **insurance glossary & analytics knowledge base**  
- Query relevance filtering (rejects irrelevant/non-insurance queries)  
- Iterative SQL repair loop (retries wrong/failing SQL)  
- Streamlit-based conversational interface  
- Caching + query history for faster responses  
- Hooks for visualization + insights agents (bar, pie, anomaly detection, narratives)  

---

## Future Improvements & Scope  
- **Multi-Cloud & Multi-DB Federation**: Query across Snowflake, Redshift, BigQuery, Databricks.  
- **Semantic Layer**: Map business terms → columns across DBs (handles schema drift).  
- **Predictive Insights**: Forecasting and trend analysis beyond descriptive stats.  
- **Governance & Security**: Role-based access control, audit logs.  
- **Multi-Agent Collaboration**: Planner agent, SQL agent, validator agent, insight agent.  
- **Enterprise-Grade Deployment**: Docker/K8s, monitoring, SSO integration.  

---


