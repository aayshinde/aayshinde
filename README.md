<h1 align="center">Ayush Shinde</h1>
<p align="center"><b>AI / ML Engineer</b> · predictive maintenance · fraud &amp; anomaly detection · LLM agents &amp; evaluation</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776ab?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/PyTorch-ee4c2c?logo=pytorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/XGBoost-1f77b4" alt="XGBoost">
  <img src="https://img.shields.io/badge/scikit--learn-f7931e?logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/LangChain%20%7C%20LangGraph-1c3c3c" alt="LangChain and LangGraph">
  <img src="https://img.shields.io/badge/PySpark%20%7C%20Databricks-e25a1c?logo=apachespark&logoColor=white" alt="PySpark and Databricks">
  <img src="https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/Docker-2496ed?logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/AWS%20%7C%20Azure-232f3e?logo=amazonwebservices&logoColor=white" alt="AWS and Azure">
</p>

I build machine-learning systems that have to be **trusted, not just accurate**: honest evaluation (time-based splits,
baselines, ablations), and models that say when they are unsure. ML Engineer at JPMorgan Chase (fraud models and data
pipelines), previously at Siemens (predictive maintenance on IoT telemetry, MLOps). M.S. in Data Science, UT Arlington.

## Featured projects

### 🛠️ [Predictive Failure &amp; Root-Cause Agent](https://github.com/aayshinde/failure-rca-agent) &nbsp;·&nbsp; [▶ live demo](https://aayshinde.github.io/failure-rca-agent/)
Predicts which machines will fail in the next 24 hours, then a LangGraph agent explains *why*, citing its evidence.

<p align="center"><a href="https://aayshinde.github.io/failure-rca-agent/"><img src="https://raw.githubusercontent.com/aayshinde/failure-rca-agent/main/docs/img/demo.gif" width="720" alt="Interactive fleet reliability console"></a></p>

- Catches **85% of 462 held-out failures with a median 20 h of warning** and 0.18 false alerts per machine per month
- LangGraph workflow vs ReAct baseline on a free local LLM: retrieval hit rate **27% → 92%**, unsupported claims **15.6% → 3.1%**
- Reports what did *not* work too: a linear baseline ties XGBoost on NASA C-MAPSS, and the agent regressed on risk questions
- `XGBoost` `PyTorch LSTM` `LangGraph` `FAISS` `FastAPI` `GitHub Actions`

### 🎫 [RAG Support Insights &amp; LLM Evaluation](https://github.com/aayshinde/rag-support-insights) &nbsp;·&nbsp; [▶ live demo](https://aayshinde.github.io/rag-support-insights/)
Support-ticket triage with retrieval and a two-stage abstention gate that **escalates to a human when the evidence is weak**,
with baselines, stress tests and failure analysis.
- `LangChain` `FAISS` `FastAPI` `Streamlit` `Ollama`

## How I work

- **Measure honestly.** Time-based splits, a strong simple baseline before a complex model, ablations, confidence intervals, and a README section for limitations.
- **Ship it.** Tests that run offline, CI, containers, and a demo anyone can open without installing anything.
- **Know when to abstain.** Systems that hand off to a person are more useful than ones that guess confidently.

## Toolbox

| | |
|---|---|
| **ML** | XGBoost · PyTorch · scikit-learn · LSTM / time-series · anomaly detection · feature engineering |
| **LLM &amp; agents** | RAG · LangChain · LangGraph · FAISS · evaluation harnesses · local models via Ollama |
| **Data** | Python · SQL · PySpark · Databricks · Spark on EMR · PostgreSQL · Snowflake |
| **MLOps** | Docker · GitHub Actions · MLflow · AWS (S3, SageMaker, EMR) · Azure (AKS) · model validation |
