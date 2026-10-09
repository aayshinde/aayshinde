<h1 align="center">Ayush Shinde</h1>
<p align="center"><b>AI / ML Engineer</b><br>
GenAI and classical ML for financial services and manufacturing · RAG · anomaly detection · honest evaluation</p>

<p align="center">
  <a href="https://aayshinde.github.io/"><img src="https://img.shields.io/badge/Portfolio-aayshinde.github.io-111827?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://www.linkedin.com/in/ayush-shinde-70295b344/"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:ayush.s@itjobinbox.com"><img src="https://img.shields.io/badge/Email-ayush.s%40itjobinbox.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/aayshinde/aayshinde/blob/main/Ayush_Shinde_Resume.pdf"><img src="https://img.shields.io/badge/Resume-PDF-2563EB?style=for-the-badge&logo=readme&logoColor=white" alt="Resume"></a>
  <a href="https://aayshinde.github.io/failure-rca-agent/"><img src="https://img.shields.io/badge/Live%20demo-failure%20agent-6ea8ff?style=for-the-badge" alt="Live demo"></a>
  <a href="https://aayshinde.github.io/rag-support-insights/"><img src="https://img.shields.io/badge/Live%20demo-RAG%20triage-b18cff?style=for-the-badge" alt="Live demo"></a>
  <a href="https://trialscope-6ysgwfp6gstc7h7v8gxkan.streamlit.app/"><img src="https://img.shields.io/badge/Live%20demo-clinical%20trials-2f6fed?style=for-the-badge" alt="Live demo"></a>
</p>

---

## About me

I'm an AI/ML engineer who cares less about a headline metric and more about whether a system holds up when someone relies on it.

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
    <td align="center"><b>2.7×</b><br><sub>more clinical-trial failures caught in the riskiest 10% than chance</sub></td>
  </tr>
</table>

<sub>The clinical-trial figure is from <a href="https://github.com/aayshinde/trialscope">TrialScope</a>, tested on years the model never saw. It uses a snapshot of live registry data, so a re-run will differ slightly.</sub>

## Featured projects

### 🛠️ Predictive Failure &amp; Root-Cause Agent &nbsp;[code](https://github.com/aayshinde/failure-rca-agent) · [**▶ try it live**](https://aayshinde.github.io/failure-rca-agent/)

> **In 30 seconds:** an early-warning system for factory machines. It warns the maintenance team about a day before a machine breaks, and when one does break, an AI assistant explains the most likely cause and shows the evidence.

- **The problem:** unplanned breakdowns are expensive, and the clues are scattered across sensor readings, error logs and repair manuals.
- **What I built:** models that watch 100 machines (simulated) and flag the ones likely to fail in the next 24 hours, plus an AI agent that investigates a failure by pulling the sensor data, the error log and the right manual pages, then answers with citations.
- **The result:** it catches 85% of failures with about 20 hours of notice and few false alarms (0.18 per machine per month). The AI agent's answers are more often backed by evidence than a simpler version's.

<p align="center"><a href="https://aayshinde.github.io/failure-rca-agent/"><img src="https://raw.githubusercontent.com/aayshinde/failure-rca-agent/main/docs/img/demo.gif" width="720" alt="Interactive fleet reliability console"></a></p>

**Stack:** XGBoost · PyTorch LSTM autoencoder · LangGraph · FAISS · FastAPI · GitHub Actions · Ollama (free local LLM)

### 🎫 RAG Support Insights &amp; LLM Evaluation &nbsp;[code](https://github.com/aayshinde/rag-support-insights) · [**▶ try it live**](https://aayshinde.github.io/rag-support-insights/)

> **In 30 seconds:** an AI helper for customer-support teams. It reads a new ticket, finds similar past tickets and how they were solved, and suggests the next step. If it isn't confident, it hands the ticket to a person instead of guessing.

- **The problem:** support agents spend time hunting for how similar issues were handled, and an AI that guesses wrong makes things worse.
- **What I built:** a search over 48,178 past tickets that classifies the new issue and recommends an action based on how similar tickets were resolved, with a two-stage check that sends weak-evidence cases to a human.
- **The result:** 91.4% correct on the tickets it answers (87% of queries), and 98% of out-of-scope messages escalated to a human instead of answered, measured on held-out tickets.

<p align="center"><a href="https://aayshinde.github.io/rag-support-insights/"><img src="https://raw.githubusercontent.com/aayshinde/aayshinde/main/docs/rag-demo.gif" width="720" alt="Walkthrough of the RAG triage demo: the answer-or-escalate flow, the confidence threshold trade-off, and an example ticket that is escalated to a human"></a></p>

**Stack:** LangChain · FAISS · FastAPI · Streamlit · Ollama

### 🧪 TrialScope: Clinical-Trial Risk Prediction &nbsp;[code](https://github.com/aayshinde/trialscope) · [**▶ try it live**](https://trialscope-6ysgwfp6gstc7h7v8gxkan.streamlit.app/)

> **In 30 seconds:** a tool that looks at a clinical trial the day it starts and estimates how likely it is to be stopped early or run late, then shows why. You can even edit a trial's eligibility rules and watch the estimate move.

- **The problem:** trials that stop early or drag on cost sponsors a great deal, and the warning signs are buried in registry text.
- **What I built:** a data pipeline over 30,000 real ClinicalTrials.gov trials, models that score each trial using only what was known when it started, and a dashboard with explanations, a what-if tool and a plain-English assistant that runs free on a local model.
- **The result:** 0.71 AUROC on 2017-2019 trials it never saw (a simple baseline gets 0.64), and the riskiest 10% of trials hold 27% of the eventual failures. A deliberately leaky version scores 0.82, which I show to explain why that number would mislead. It is a ranking aid, not a forecast for any single trial.

<p align="center"><a href="https://trialscope-6ysgwfp6gstc7h7v8gxkan.streamlit.app/"><img src="https://raw.githubusercontent.com/aayshinde/trialscope/main/docs/img/overview.png" width="720" alt="TrialScope dashboard overview"></a></p>

**Stack:** XGBoost · lifelines · SHAP · dbt · DuckDB · Prefect · MLflow · LangGraph · Streamlit · Ollama (free local LLM)

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
<img src="https://img.shields.io/badge/Survival%20analysis-444?style=flat" alt="Survival%20analysis">
<img src="https://img.shields.io/badge/SHAP%20explainability-444?style=flat" alt="SHAP%20explainability">
<img src="https://img.shields.io/badge/Probability%20calibration-444?style=flat" alt="Probability%20calibration">
<img src="https://img.shields.io/badge/Leakage-safe%20validation-444?style=flat" alt="Leakage-safe%20validation">

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
<img src="https://img.shields.io/badge/Ollama%20(local%20LLMs)-000?style=flat&logo=ollama&logoColor=white" alt="Ollama%20(local%20LLMs)">

**Data engineering**<br>
<img src="https://img.shields.io/badge/Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white" alt="Airflow">
<img src="https://img.shields.io/badge/Spark-E25A1C?style=flat&logo=apachespark&logoColor=white" alt="Spark">
<img src="https://img.shields.io/badge/Kafka-231F20?style=flat&logo=apachekafka&logoColor=white" alt="Kafka">
<img src="https://img.shields.io/badge/AWS%20EMR-232F3E?style=flat&logo=amazonwebservices&logoColor=white" alt="AWS%20EMR">
<img src="https://img.shields.io/badge/dbt-FF694B?style=flat&logo=dbt&logoColor=white" alt="dbt">
<img src="https://img.shields.io/badge/DuckDB-FFF000?style=flat&logo=duckdb&logoColor=black" alt="DuckDB">
<img src="https://img.shields.io/badge/Prefect-070E10?style=flat&logo=prefect&logoColor=white" alt="Prefect">
<img src="https://img.shields.io/badge/Data-quality%20tests-444?style=flat" alt="Data-quality%20tests">

**MLOps & deployment**<br>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=flat&logo=mlflow&logoColor=white" alt="MLflow">
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker">
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white" alt="Kubernetes">
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white" alt="FastAPI">
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat&logo=githubactions&logoColor=white" alt="GitHub%20Actions">
<img src="https://img.shields.io/badge/Jenkins-D24939?style=flat&logo=jenkins&logoColor=white" alt="Jenkins">
<img src="https://img.shields.io/badge/Weights%20%26%20Biases-FFBE00?style=flat&logo=weightsandbiases&logoColor=white" alt="Weights%20%26%20Biases">
<img src="https://img.shields.io/badge/Drift%20monitoring-444?style=flat" alt="Drift%20monitoring">
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white" alt="Streamlit">

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

Open to talking about ML systems, evaluation, and fraud, predictive-maintenance or clinical-trial risk problems.
**[Portfolio](https://aayshinde.github.io/)** · **[LinkedIn](https://www.linkedin.com/in/ayush-shinde-70295b344/)** · **[Email](mailto:ayush.s@itjobinbox.com)** · **[Resume](https://github.com/aayshinde/aayshinde/blob/main/Ayush_Shinde_Resume.pdf)**
