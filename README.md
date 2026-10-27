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

### American Airlines Market Demand Forecasting | Capstone with AA Network Planning (UNT, Fall 2026)
Python · LightGBM · statsforecast · NeuralForecast · Chronos · pandas · Snowflake

- Forecast monthly origin–destination passenger demand, revenue and average fare 1–24 months ahead for every airport-pair market in American Airlines' network-planning data, summed bottom-up to station, region and network totals: the horizon on which schedules (on sale 330 days out) and long-haul capacity are committed.
- Benchmarked the full model landscape against a seasonal-naive baseline on four rolling, time-ordered forecast origins. Per-route ARIMA/ETS/Theta, tuned N-BEATSx and TFT, and zero-shot foundation models (Chronos-2, TimesFM, TiRex, Toto) all failed to beat it; one global LightGBM with horizon-aware training rows, absolute-error loss and a recent-origins training window did.
- Final model blends LightGBM (0.35) with a three-year seasonal average on COVID-repaired history (0.65), weighted down from 50/50 because the tree model's bias compounds when markets are summed. It cut MASE by 9.3% vs. the benchmark for passengers, 10.8% for revenue and 14.9% for fare, and won at every hierarchy level, region and horizon.
- Split-conformal 80%/50% prediction intervals validated level by level (81.5% coverage for markets); region and network intervals were withheld after failing validation. Features were accepted only above a random-probe noise floor, two target leaks were found and closed, and a route-level event study showed a Super Bowl effect concentrated on the competing teams' routes and invisible at airport level. Every number in the paper is generated from pipeline outputs and reproduced from a clean rebuild. Code is private: the sponsor's data is under NDA.

### [Biohub Cell Tracking Tooling](https://github.com/unt-akanksha/biohub-cell-tracking-competition) | ML competition infrastructure
Python · Kaggle CLI

- Built an offline-first control plane for a Kaggle cell-tracking competition: a CLI that snapshots live competition state and keeps an immutable experiment registry.
- Enforces a fail-closed GPU workflow (register → preflight → authorize → execute → watchdog) with a protected GPU-hours reserve, and statically audits top public leaderboard notebooks for known exploits before treating them as clean.

### [LLM Fund-Selection Bias](https://github.com/unt-akanksha/llm-fund-bias) | Behavioral experiment on LLM agents
Python · OpenAI & Anthropic APIs · Ollama · pandas · statsmodels · SciPy · matplotlib · pytest

- Designed an experiment testing whether persuasive documents (brand popularity, a fabricated expert survey, past performance) push LLM agents from the cheaper of two same-index ETFs to a costlier one, using verified issuer fact-sheet data (S&P 500: SPY/IVV/VOO; Nasdaq-100: QQQ/QQQM) and cost regret in basis points as ground truth.
- Ran 11,200 seeded, logged calls across 8 models from 3 families (OpenAI gpt-5.4 nano/mini/full, Anthropic Claude Haiku/Sonnet/Opus 5.5, local Qwen 2.5 7B/14B), crossing 5 contexts × 2 prompt templates × 2 system prompts (standard vs fiduciary). Built a multi-provider runner with hard spend caps ($18.50 total API cost), resumable logs, a design frozen before the runs, and a quality gate with manual review.
- Found that baseline quality and robustness diverge: gpt-5.4-nano and mini chose the cheaper fund without context but switched to the costlier one in up to 98–100% of picks after one persuasive document; Qwen favored the costlier Nasdaq-100 fund even without one (58–81%); gpt-5.4 and all three Claude models never switched. A one-sentence fiduciary instruction cut persuasion by 18–45 points for some models and had no effect on others.
- Reported risk differences with Newcombe confidence intervals and one-sided Fisher tests with Holm correction, plus robustness checks (same effect direction across templates in 47 of 48 contrasts; matched 30-run comparison). Earlier iterations (fictional funds; 13 real ETFs) and a source-checked literature review on persuasion, sycophancy and fiduciary rules are in the repo.

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

- Compared a CNN trained from scratch with ResNet50 transfer learning across five skin-condition classes. Found that the published 9,548-image dataset was 341 photos × 28 pre-made augmentations, so splitting by file would leak every validation photo into training.
- After splitting by source photo and fixing ResNet50's input preprocessing, ResNet50 reached 85.9% test accuracy (macro-F1 0.85) on 52 held-out photos vs. 55.9% for the from-scratch CNN. Academic project, not a clinical tool.

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
