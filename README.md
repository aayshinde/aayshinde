<h1 align="center">Ayush Shinde</h1>
<p align="center"><b>AI / ML Engineer</b><br>
GenAI and classical ML for financial services and manufacturing · RAG · anomaly detection · honest evaluation</p>

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

- 🏦 **Now:** AI/ML Engineer at **JPMorgan Chase**: contributing to a RAG assistant over internal policy documentation (AWS Bedrock, OpenSearch) with ownership of retrieval evaluation and chunking, tuning gradient-boosted anomaly and risk classifiers with assumptions documented for Model Risk review, and building PySpark feature pipelines on EMR with Airflow and MLflow
- 🏭 **Before:** ML Engineer at **Siemens**: predictive-maintenance models (LSTM, XGBoost) on industrial IoT telemetry, PySpark pipelines, containerized real-time inference on Azure AKS, and CI/CD for model releases
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

## Skills

**Programming & data**<br>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
<img src="https://img.shields.io/badge/SQL-336791?style=flat&logo=postgresql&logoColor=white" alt="SQL">
<img src="https://img.shields.io/badge/PySpark-E25A1C?style=flat&logo=apachespark&logoColor=white" alt="PySpark">
<img src="https://img.shields.io/badge/Bash-4EAA25?style=flat&logo=gnubash&logoColor=white" alt="Bash">
<img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white" alt="Git">

**Machine learning**<br>
<img src="https://img.shields.io/badge/XGBoost-1f77b4?style=flat" alt="XGBoost">
<img src="https://img.shields.io/badge/LightGBM-2E8B57?style=flat" alt="LightGBM">
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white" alt="scikit--learn">
<img src="https://img.shields.io/badge/Time--series-444?style=flat" alt="Time--series">
<img src="https://img.shields.io/badge/Feature%20engineering-444?style=flat" alt="Feature%20engineering">
<img src="https://img.shields.io/badge/Model%20evaluation-444?style=flat" alt="Model%20evaluation">

**Deep learning**<br>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white" alt="PyTorch">
<img src="https://img.shields.io/badge/TensorFlow%20%2F%20Keras-FF6F00?style=flat&logo=tensorflow&logoColor=white" alt="TensorFlow%20%2F%20Keras">
<img src="https://img.shields.io/badge/LSTM-444?style=flat" alt="LSTM">
<img src="https://img.shields.io/badge/Transformers-444?style=flat" alt="Transformers">
<img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=white" alt="Hugging%20Face">

**Generative AI & LLMs**<br>
<img src="https://img.shields.io/badge/RAG-111827?style=flat" alt="RAG">
<img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat" alt="LangChain">
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat" alt="LangGraph">
<img src="https://img.shields.io/badge/LoRA%20%2F%20QLoRA-444?style=flat" alt="LoRA%20%2F%20QLoRA">
<img src="https://img.shields.io/badge/FAISS-0467DF?style=flat" alt="FAISS">
<img src="https://img.shields.io/badge/OpenSearch-005EB8?style=flat&logo=opensearch&logoColor=white" alt="OpenSearch">
<img src="https://img.shields.io/badge/Pinecone-000?style=flat&logo=pinecone&logoColor=white" alt="Pinecone">
<img src="https://img.shields.io/badge/LLM%20evaluation-444?style=flat" alt="LLM%20evaluation">

**Data engineering**<br>
<img src="https://img.shields.io/badge/Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white" alt="Airflow">
<img src="https://img.shields.io/badge/Spark-E25A1C?style=flat&logo=apachespark&logoColor=white" alt="Spark">
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white" alt="Kafka">
<img src="https://img.shields.io/badge/AWS%20EMR-232F3E?style=flat&logo=amazonwebservices&logoColor=white" alt="AWS%20EMR">

**MLOps & deployment**<br>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat&logo=mlflow&logoColor=white" alt="MLflow">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white" alt="Kubernetes">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white" alt="GitHub%20Actions">
<img src="https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white" alt="Jenkins">
<img src="https://img.shields.io/badge/Weights%20%26%20Biases-FFBE00?style=flat&logo=weightsandbiases&logoColor=white" alt="Weights%20%26%20Biases">
<img src="https://img.shields.io/badge/Drift%20monitoring-444?style=flat" alt="Drift%20monitoring">

**Cloud**<br>
<img src="https://img.shields.io/badge/AWS%20Bedrock%20%7C%20SageMaker-232F3E?style=flat&logo=amazonwebservices&logoColor=white" alt="AWS%20Bedrock%20%7C%20SageMaker">
<img src="https://img.shields.io/badge/S3%20%7C%20EMR%20%7C%20Lambda-232F3E?style=flat&logo=amazonwebservices&logoColor=white" alt="S3%20%7C%20EMR%20%7C%20Lambda">
<img src="https://img.shields.io/badge/Azure%20ML-0078D4?style=flat&logo=microsoftazure&logoColor=white" alt="Azure%20ML">

## Certifications

| Certification | Issuer | Verify |
|---|---|---|
| 🏅 **Certified Associate Machine Learning Engineer** | AWS | [Credly](https://www.credly.com/badges/f96d98cb-5acc-4b20-ab3c-034d012a3d2d/public_url) |
| 🏅 **Databricks Fundamentals** | Databricks | [Credential](https://credentials.databricks.com/ddbfc573-f0e5-4317-b799-303ea144794e#acc.69rFtHwN) |
| 🏅 **Advanced Google Data Analytics** | Google | [Coursera](https://www.coursera.org/account/accomplishments/verify/S585E7EF9J2L) |

## Let's connect

Open to talking about ML systems, evaluation, and fraud or predictive-maintenance problems.
**[LinkedIn](https://www.linkedin.com/in/ayush-shinde-70295b344/)** · **[Email](mailto:ayush.s@itjobinbox.com)** · **[Resume](https://github.com/aayshinde/aayshinde/blob/main/Ayush_Shinde_Resume.pdf)**
