# Hey, I'm Praveen 👋

I'm a Gen AI/ML Engineer based in Georgia, with about four years now of building machine
learning and generative AI systems for banking and fintech — environments where "it works
on my laptop" isn't good enough, because the moment compliance, audit trails, and risk
controls get involved, everything has to be production-grade from day one.

Right now I'm at Citibank, where I work on the Gen AI platform supporting our Chief
Investment Office — basically helping 300+ analysts, portfolio managers, and compliance
folks get through regulatory analysis and investment research faster without cutting
corners on accuracy. Before that, I spent a couple of years at LTI Mindtree, where I got
my hands dirty across fraud detection, churn prediction, and forecasting for fintech
clients — which is honestly where I learned that a model's accuracy on a holdout set means
nothing if nobody can explain why it made a decision.

These days most of my time goes into the things that make GenAI systems actually trustworthy:
retrieval-augmented generation, multi-agent systems, fine-tuning open models on financial
text, and the unglamorous but critical MLOps/LLMOps work that keeps all of it from quietly
drifting into garbage in production.

---

## What I actually do day to day

**Building RAG systems that don't hallucinate confidently wrong answers.**
I've spent a lot of time on the retrieval side — chunking strategy, embedding choice,
reranking — because in finance, a wrong answer delivered confidently is worse than no
answer. My current RAG pipeline (FAISS + Redis) improved retrieval relevance by 35% over
our earlier version, mostly by getting more disciplined about reranking instead of just
throwing more documents at the LLM.

**Designing multi-agent workflows.**
I built a multi-agent system using LangGraph and MCP where separate agents handle research,
compliance verification, and reporting — with tool use and self-reflection loops so agents
can catch their own mistakes before they reach a human. That cut manual regulatory review
effort by about half on the workflows it touches.

**Fine-tuning LLMs without melting a GPU budget.**
I've fine-tuned domain-specific models (FinGPT, Palmyra) using QLoRA and PEFT for
summarizing and classifying regulatory text. The appeal of QLoRA isn't just that it works —
it's that it cut our GPU memory footprint by 60%, which matters a lot when you're not
working with unlimited compute.

**Keeping production systems honest.**
None of the above matters if it silently degrades over time. I've set up MLflow + Airflow
pipelines for automated retraining and drift detection, and built evaluation gates using
ROUGE scoring and finance-specific accuracy checks directly into GitHub Actions, so a bad
model change gets blocked before it ships, not after someone notices the outputs got worse.

---

## Tech I work with regularly

**Languages:** Python (daily driver), SQL, Java, Scala, R, Bash

**ML/DL:** Scikit-learn, XGBoost, LightGBM, PyTorch, TensorFlow/Keras, LSTM, CNN,
Hugging Face Transformers

**GenAI/LLM stack:** GPT-4/4o, Claude, LLaMA, Mistral, Gemini, LangChain, LangGraph,
LlamaIndex, RAG, PEFT/QLoRA/LoRA, prompt engineering, agentic workflows, function calling

**MLOps/LLMOps:** MLflow, Weights & Biases, DVC, Docker, Kubernetes, drift monitoring,
model governance, A/B testing, BentoML

**Cloud:** AWS (SageMaker, EC2, S3, Lambda, Bedrock), Azure (Azure ML, Databricks, OpenAI
Service), GCP (Vertex AI, BigQuery)

**APIs & architecture:** REST, MCP (Model Context Protocol), FastAPI, Flask, GraphQL,
WebSockets

**Data & vector stores:** PostgreSQL, MySQL, MongoDB, Pinecone, Weaviate, FAISS, Redis,
ChromaDB

**Big data & pipelines:** Apache Spark, Kafka, Airflow, dbt, Great Expectations

**Evaluation & explainability:** SHAP, LIME, ROUGE, BERTScore, Perplexity, ROC-AUC,
cross-validation

---

## A couple of projects I'm proud of

### 📑 Financial Document Intelligence System
A RAG platform I built to make SEC filings and financial reports actually queryable in
plain English instead of forcing someone to dig through a 200-page 10-K manually. It
handles the full pipeline — document ingestion, chunking, embedding generation, vector
search, and generation — and returns answers grounded in the actual source documents
rather than the model just making things up. Built with Python, LangChain, and vector
databases.

### 📈 Real-Time Stock Sentiment & Trading Signal Engine
A pipeline that ingests live financial news and Reddit chatter through Kafka and PySpark,
processing 10,000+ signals a day. I fine-tuned FinBERT to classify sentiment on earnings
calls and analyst reports (93% F1 on held-out data), then combined that with an LSTM +
XGBoost ensemble to predict short-term price movement — it beat the baseline by 22%.
Deployed as a FastAPI service on AWS Lambda, serving predictions in under 100ms with
MLflow tracking drift in the background.

---

## Background

🎓 **Master of Science in Computer Science** — Kent State University, OH

📜 **Certifications:**
- Anthropic: Claude 101
- Anthropic AI Fluency: Framework & Foundation
- Microsoft Certified: Azure Developer Associate
- Oracle: Database PL/SQL Developer Certified Professional

---

## Let's talk

If you're working on anything involving RAG, agentic systems, or applying GenAI in
regulated industries, I'd genuinely enjoy comparing notes.

📧 Praveen.b@mycvhire.com
💼 linkedin.com/in/praveenkumarbotta
📍 Georgia, USA

*Open to GenAI, ML Engineering, and AI platform roles.*
