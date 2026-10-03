<h1 align="center">Ayush Shinde</h1>
<p align="center"><b>AI / ML Engineer</b><br>
Models you can trust: predictive maintenance · fraud &amp; anomaly detection · LLM agents with honest evaluation</p>

<p align="center">
  <a href="https://www.linkedin.com/in/ayush-shinde-70295b344/"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:ayush.s@itjobinbox.com"><img src="https://img.shields.io/badge/Email-ayush.s%40itjobinbox.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/aayshinde/aayshinde/blob/main/Ayush_Shinde_Resume.pdf"><img src="https://img.shields.io/badge/Resume-PDF-2563EB?style=for-the-badge&logo=readme&logoColor=white" alt="Resume"></a>
  <a href="https://aayshinde.github.io/failure-rca-agent/"><img src="https://img.shields.io/badge/Live%20demo-failure%20agent-6ea8ff?style=for-the-badge" alt="Live demo"></a>
  <a href="https://aayshinde.github.io/rag-support-insights/"><img src="https://img.shields.io/badge/Live%20demo-RAG%20triage-b18cff?style=for-the-badge" alt="Live demo"></a>
</p>

---

## About me

I'm an ML engineer who cares less about a headline metric and more about whether a system holds up when someone relies on it.

- 🏦 **Now:** ML Engineer at **JPMorgan Chase**, building fraud classification models and the data pipelines behind them, and working with fraud analysts and model-risk teams to review false positives and support controlled model releases
- 🏭 **Before:** ML Engineer at **Siemens**, building predictive-maintenance models on industrial IoT telemetry, PySpark pipelines, containerized real-time inference and CI/CD for model releases
- 🎓 **Education:** M.S. Data Science, University of Texas at Arlington (2026) · B.E. Electronics &amp; Telecommunication, AI &amp; ML Honors, University of Mumbai
- 🔬 **What I'm exploring:** LLM agents that cite their evidence, evaluation that reports failures honestly, and systems that abstain instead of guessing
- 📍 Based in Texas

## Proof, not promises

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

## Featured projects

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

## Skills

**Languages & data**<br>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/SQL-336791?style=flat&logo=postgresql&logoColor=white" alt="SQL">
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat&logo=apachespark&logoColor=white" alt="PySpark">
<img src="https://img.shields.io/badge/Scala-DC322F?style=flat&logo=scala&logoColor=white" alt="Scala">
<img src="https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white" alt="Bash">
<img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" alt="Pandas">
<img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" alt="NumPy">

**Machine learning**<br>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" alt="PyTorch">
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white" alt="TensorFlow">
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white" alt="scikit--learn">
<img src="https://img.shields.io/badge/XGBoost-1f77b4?style=flat" alt="XGBoost">
<img src="https://img.shields.io/badge/LSTM%20%2F%20time--series-444?style=flat" alt="LSTM%20%2F%20time--series">
<img src="https://img.shields.io/badge/Anomaly%20detection-444?style=flat" alt="Anomaly%20detection">

**LLM systems**<br>
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat" alt="LangChain">
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat" alt="LangGraph">
<img src="https://img.shields.io/badge/RAG-111827?style=flat" alt="RAG">
<img src="https://img.shields.io/badge/FAISS-0467DF?style=flat" alt="FAISS">
<img src="https://img.shields.io/badge/Ollama-111111?style=flat&logo=ollama&logoColor=white" alt="Ollama">
<img src="https://img.shields.io/badge/LLM%20evaluation-444?style=flat" alt="LLM%20evaluation">

**Data platforms & cloud**<br>
<img src="https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white" alt="Databricks">
<img src="https://img.shields.io/badge/Spark%20%2F%20EMR-E25A1C?style=flat&logo=apachespark&logoColor=white" alt="Spark%20%2F%20EMR">
<img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white" alt="AWS">
<img src="https://img.shields.io/badge/Azure-0078D4?style=flat&logo=microsoftazure&logoColor=white" alt="Azure">
<img src="https://img.shields.io/badge/Snowflake-29B5E8?style=flat&logo=snowflake&logoColor=white" alt="Snowflake">
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" alt="PostgreSQL">
<img src="https://img.shields.io/badge/Tableau-E97627?style=flat&logo=tableau&logoColor=white" alt="Tableau">

**MLOps & serving**<br>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white" alt="Kubernetes">
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white" alt="GitHub%20Actions">
<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat&logo=mlflow&logoColor=white" alt="MLflow">
<img src="https://img.shields.io/badge/CI%2FCD-444?style=flat" alt="CI%2FCD">

## Certifications

| Certification | Issuer | Verify |
|---|---|---|
| 🏅 **Certified Associate Machine Learning Engineer** | AWS | [Credly](https://www.credly.com/badges/f96d98cb-5acc-4b20-ab3c-034d012a3d2d/public_url) |
| 🏅 **Databricks Fundamentals** | Databricks | [Credential](https://credentials.databricks.com/ddbfc573-f0e5-4317-b799-303ea144794e#acc.69rFtHwN) |
| 🏅 **Advanced Google Data Analytics** | Google | [Coursera](https://www.coursera.org/account/accomplishments/verify/S585E7EF9J2L) |

## Let's connect

Open to talking about ML systems, evaluation, and fraud or predictive-maintenance problems.
**[LinkedIn](https://www.linkedin.com/in/ayush-shinde-70295b344/)** · **[Email](mailto:ayush.s@itjobinbox.com)** · **[Resume](https://github.com/aayshinde/aayshinde/blob/main/Ayush_Shinde_Resume.pdf)**
