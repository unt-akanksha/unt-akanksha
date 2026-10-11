<h1 align="center">Akanksha Tiwari</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Student%20at%20UNT-Data%20Science%20%7C%20Statistics%20%7C%20Analytics-0A66C2" alt="Student at UNT" />
  <img src="https://img.shields.io/badge/Location-Dallas%2C%20Texas-FF6B6B" alt="Location" />
</p>

<p align="center">
  <em>Graduate student in data analytics and operations research, transitioning toward AI engineering with a focus on machine learning systems, LLM workflows, and decision-support applications.</em>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/akanksha-tiwari-2803"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white" /></a>
  <a href="mailto:akankshat2803@gmail.com"><img src="https://img.shields.io/badge/Email-akankshat2803%40gmail.com-D14836?logo=gmail&logoColor=white" /></a>
</p>

---

## About Me

Graduate student at the University of North Texas with a strong foundation in statistics, operational research, and applied data science. I am actively transitioning toward AI engineering, with interest in machine learning systems, LLM-based workflows, retrieval and recommendation systems, and production-grade AI applications.

My background includes forecasting, multimodal retrieval, experimentation, marketing mix modeling, and optimization — with prior industry experience as a Senior Research Data Scientist and current work as a Teaching Assistant for Applied Statistics.

---

## Core Strengths

- Machine learning system design and deployment
- Forecasting and demand modeling
- Recommendation systems and personalization
- NLP, embeddings, and multimodal retrieval
- Marketing Mix Modeling (MMM) and media-efficiency analysis
- A/B testing, experimentation, and incrementality
- Causal inference and decision science
- Optimization and allocation modeling
- Generative AI, RAG, and model evaluation
- AI product thinking and practical ML engineering

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-FF6C37?style=for-the-badge&logo=apache-spark&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=for-the-badge&logo=apache-airflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![SageMaker](https://img.shields.io/badge/SageMaker-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)

---

## Selected Impact

### Teaching Assistant | University of North Texas
Aug 2026 - Present

- Teaching Assistant for Applied Statistics for undergraduate students.
- Support students in statistical modeling, forecasting, experimental design, and scientific communication.
- Help bridge theoretical concepts with practical analytical reasoning and real-world data applications.

### Senior Research Data Scientist | dunnhumby
Jul 2022 - Nov 2025

- Built econometric and LSTM forecasting models on 10M+ transactions to quantify national-media drivers and forecast spend.
- Developed Long-term Multichannel Modeling using an ML-first Marketing Mix Modeling framework to uncover channel characteristics and guide medium- to long-term marketing investments.
- Built multimodal retrieval using ResNet and BERT embeddings, improving mAP by 18% and CTR by 8%.
- Productionized PySpark scoring for 5M+ customer-product pairs, reducing batch time by 40%.
- Built a FastText substitution engine that improved recommendation accuracy by 22%.
- Designed segmentation frameworks using K-means, hierarchical clustering, and event-based purchase triggers.
- Created a PuLP-based coupon-allocation model across 50+ product categories, contributing $2M+ in incremental revenue.
- Evaluated next-generation recommender systems including SASRec, SAR, and ALS through hyperparameter tuning and A/B testing.

### Data Analyst | Merkle (Dentsu)
Aug 2021 - Oct 2021

- Analyzed multi-year campaign data to identify behavior patterns and define six high-value customer segments.
- Built Python and SQL pipelines with validation checks to achieve 99.5% data accuracy.

---

## Projects

### [Biohub Cell Tracking Tooling](https://github.com/unt-akanksha/biohub-cell-tracking-competition) | ML competition infrastructure
Python · Kaggle CLI

- Built an offline-first control plane for a Kaggle cell-tracking competition: a CLI that snapshots live competition state and keeps an immutable experiment registry.
- Enforces a fail-closed GPU workflow (register → preflight → authorize → execute → watchdog) with a protected GPU-hours reserve, and statically audits top public leaderboard notebooks for known exploits before treating them as clean.

### [LLM Fund-Selection Bias](https://github.com/unt-akanksha/llm-fund-bias) | Behavioral experiment on LLM agents
Python · Ollama · pandas · statsmodels · pytest

- Designed a controlled experiment testing whether injected documents and user-memory statements pull LLM agents away from an objectively dominant fund, adapting Wharton's agentic-shopping study design to finance.
- Ran 2,200 logged, reproducible model calls on two local open models (Llama 3.1 8B, Qwen 2.5 7B), with seeded shuffling, resumable append-only logs, a design frozen before the main runs, and 0% parse failures.
- Found that a single ~200-word document moved 93–100% of picks to the fund it recommended, and one sentence of user memory ("I love tech companies!") moved 98–100% to a high-fee tech fund. Without context, 75–86% of picks went to the dominant fund.
- Estimated effects with Wilson confidence intervals, linear probability models with HC3 robust standard errors, and chi-square tests. A confirmatory order test showed that reordering the same three sources moved the dominant-fund rate from 98–99% down to as low as 41%.

### [AI Research Assistant](https://github.com/unt-akanksha/rag-research-assistant) | RAG over PDF papers
Python · Streamlit · FAISS · sentence-transformers · OpenAI-compatible LLMs · pytest

- Built a retrieval-augmented assistant that answers questions over uploaded PDFs with inline citations (file, page, chunk) and refuses out-of-scope questions through a relevance gate instead of guessing.
- Implemented page-aware chunking, hybrid vector + lexical ranking, follow-up query rewriting, summaries and multi-paper comparison. It runs with OpenAI, Groq or local Ollama models, or with no API key in extractive mode.
- Built an evaluation suite (hit rate, MRR, precision@k, context recall, groundedness, optional LLM judge). On three research papers with an 11-question test set, a chunk-size × top-k sweep raised context recall from 0.69 to 0.99. Covered by 29 offline unit tests.

### [Provenance Guard](https://github.com/unt-akanksha/Provenance-guard) | AI-generated text detection API
Python · Flask · Groq (Llama 3.3 70B) · SQLite · Flask-Limiter

- Designed a 3-signal detection ensemble (LLM classifier, stylometric heuristics, vocabulary burstiness) with documented weights and a separate weighting for short texts.
- Set confidence thresholds around the cost of falsely accusing a human writer: a wide "uncertain" band, and an AI threshold recalibrated from 0.85 to 0.78 after testing showed the original was unreachable.
- Shipped a creator appeals workflow, SQLite audit log, per-endpoint rate limits, an analytics endpoint tracking appeal rate, and a human-verification "provenance certificate".

### [TakeMeter](https://github.com/unt-akanksha/Takemeter) | Fine-tuned text classifier
Python · Hugging Face Transformers · DistilBERT · Groq · Gradio

- Fine-tuned DistilBERT to label r/nba posts as analysis, hot take or reaction, using a custom label taxonomy with written decision rules for edge cases and a 207-example dataset (LLM-generated, then reviewed against the taxonomy).
- Reached 100% accuracy on a 32-example test set vs. 78.1% for a zero-shot Llama 3.3 70B baseline, after retuning hyperparameters when the first run underperformed the baseline (68.8%).
- Error analysis showed all 7 baseline errors were the same confusion, analysis labeled as hot take, on posts citing one statistic followed by a confident conclusion.

### [Skin Disease Classification](https://github.com/unt-akanksha/Skin-Disease-Classification) | Image classification (academic)
Python · TensorFlow/Keras · scikit-learn

- Compared a CNN trained from scratch with a fine-tuned ResNet50 on 9,548 class-imbalanced images across five skin-condition classes, with data augmentation during training.
- The from-scratch CNN reached 92.3% validation accuracy vs. 57.1% for the fine-tuned ResNet50 on the same split. Academic project, not a clinical tool.

---

## Education

- Master of Science in Advanced Data Analytics, University of North Texas
- Master of Science in Operational Research, University of Delhi
- B.Sc. (Hons.) in Statistics, University of Delhi
- Certificate in Applications of AI Engineering, CodePath

Strong quantitative foundation in statistics, optimization, and decision science.

### CodePath AI Engineering Certificate

Coursework and practical exposure included:

- Python and software engineering fundamentals
- APIs, application integration, and backend workflows
- Data handling, feature pipelines, and ML development
- Prompt engineering and LLM interaction patterns
- Retrieval-augmented generation (RAG) and AI application design
- AI product thinking, evaluation, and deployment basics

---

## Research

- [RG-TTA: Regime-Guided Meta-Control for Test-Time Adaptation in Streaming Time Series](https://arxiv.org/abs/2603.27814) (arXiv:2603.27814)
- [Regime-Calibrated Fleet Repositioning with a Spatial Queue-Regret Decomposition](https://arxiv.org/abs/2604.03883) (arXiv:2604.03883)

---

## Current Focus

- AI engineering and production ML systems
- LLM workflows, retrieval, and AI application design
- Forecasting and decision systems
- MMM, media measurement, and channel optimization
- Recommendation and personalization at scale
- Multimodal AI and retrieval-based systems

---

<p align="center">
  <img src="https://img.shields.io/badge/AI%20Engineering-ML%20Systems-8A2BE2" />
  <img src="https://img.shields.io/badge/LLM-Applications%20%26%20RAG-00C7B7" />
  <img src="https://img.shields.io/badge/NLP-Embeddings%20%26%20Retrieval-FF7F50" />
  <img src="https://img.shields.io/badge/Decision%20Science-Forecasting%20%26%20MMM-6A5ACD" />
</p>

<p align="center">
  <i>Building systems that turn insight into action.</i>
</p>
