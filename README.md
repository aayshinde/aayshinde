<h1 align="center">Ayush Shinde</h1>
<p align="center"><b>AI / ML Engineer</b><br>
Models you can trust: predictive maintenance · fraud &amp; anomaly detection · LLM agents with honest evaluation</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ayush-shinde-70295b344/"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://aayshinde.github.io/failure-rca-agent/"><img src="https://img.shields.io/badge/Live%20demo-failure%20agent-6ea8ff?style=for-the-badge" alt="Live demo"></a>
  <a href="https://aayshinde.github.io/rag-support-insights/"><img src="https://img.shields.io/badge/Live%20demo-RAG%20triage-b18cff?style=for-the-badge" alt="Live demo"></a>
</p>

---

### The short version

I'm an ML engineer who cares less about a headline metric and more about whether the system holds up when someone
relies on it. At **JPMorgan Chase** I build fraud models and the data pipelines behind them; at **Siemens** I built predictive
maintenance on industrial IoT telemetry. M.S. in Data Science, UT Arlington. Based in Texas.

### Proof, not promises

Every number below is reproduced by one command in the linked repo, on a held-out test set.

<table align="center">
  <tr>
    <td align="center"><b>85%</b><br><sub>of 462 failures caught</sub></td>
    <td align="center"><b>20 h</b><br><sub>median warning before failure</sub></td>
    <td align="center"><b>0.18</b><br><sub>false alerts / machine / month</sub></td>
    <td align="center"><b>27% → 92%</b><br><sub>doc-retrieval hit rate, agent redesign</sub></td>
    <td align="center"><b>15.6% → 3.1%</b><br><sub>unsupported LLM claims</sub></td>
  </tr>
</table>

## Selected work

### 🛠️ Predictive Failure &amp; Root-Cause Agent &nbsp;[code](https://github.com/aayshinde/failure-rca-agent) · [**▶ try it live**](https://aayshinde.github.io/failure-rca-agent/)

Scores a 100-machine fleet hour by hour, warns about failures about a day ahead, then a LangGraph agent explains the
likely root cause and cites the evidence it used. Drag the clock, click a machine, replay a real failure.

<p align="center"><a href="https://aayshinde.github.io/failure-rca-agent/"><img src="https://raw.githubusercontent.com/aayshinde/failure-rca-agent/main/docs/img/demo.gif" width="720" alt="Interactive fleet reliability console"></a></p>

**Stack:** XGBoost · PyTorch LSTM autoencoder · LangGraph · FAISS · FastAPI · GitHub Actions · Ollama (free local LLM)

### 🎫 RAG Support Insights &amp; LLM Evaluation &nbsp;[code](https://github.com/aayshinde/rag-support-insights) · [**▶ try it live**](https://aayshinde.github.io/rag-support-insights/)

Triages support tickets with retrieval and a two-stage abstention gate: when the evidence is weak it **escalates to a
human instead of guessing**. Includes baselines, stress tests and failure analysis.

**Stack:** LangChain · FAISS · FastAPI · Streamlit · Ollama

## What didn't work (and what I did about it)

The projects above document their failures in the README, because that is where the engineering judgment shows.

- **A simple model matched the fancy one.** On NASA's turbofan benchmark a logistic regression tied XGBoost (AUROC 0.99). I report it and argue where the complexity does pay off.
- **My redesigned agent got worse at one task.** The LangGraph workflow beat the baseline on retrieval and grounding but missed 2 of 3 impending failures on risk questions. It is in the README, not buried.
- **My judge was the same model as my agent.** That flatters both, so the write-up says so and names the fix.

## Toolbox

| | |
|---|---|
| **Modeling** | XGBoost · PyTorch · scikit-learn · time-series (LSTM) · anomaly detection · feature engineering |
| **LLM systems** | RAG · LangChain / LangGraph · FAISS · evaluation harnesses · abstention · local models (Ollama) |
| **Data** | Python · SQL · PySpark · Databricks · Spark on EMR · PostgreSQL · Snowflake |
| **Shipping** | FastAPI · Docker · GitHub Actions · MLflow · AWS (S3, SageMaker, EMR) · Azure (AKS) |

## Experience

- **ML Engineer, JPMorgan Chase** (2026 to now): fraud classification features and models, PySpark/Databricks data pipelines with validation checks, and model-risk review of false positives.
- **ML Engineer, Siemens** (2022 to 2024): predictive maintenance with LSTM and XGBoost on IoT telemetry, PySpark pipelines, containerized real-time inference, and CI/CD for model releases.

**Education:** M.S. Data Science, University of Texas at Arlington (2026) · B.E. Electronics &amp; Telecommunication, AI &amp; ML Honors, University of Mumbai
**Certified:** [AWS Certified Associate ML Engineer](https://www.credly.com/badges/f96d98cb-5acc-4b20-ab3c-034d012a3d2d/public_url) · Databricks Fundamentals · Google Advanced Data Analytics
