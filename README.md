# 👋 Hey, I'm Yash!
**Full-Stack AI, Machine Learning & Systems Engineer**  
🎓 Actively building intelligent systems, autonomous vision pipelines & scalable web applications.  

[![GitHub](https://img.shields.io/badge/GitHub-1yash0804-181717?style=flat&logo=github)](https://github.com/1yash0804)
[![Email](https://img.shields.io/badge/Email-singhyash0804%40gmail.com-EA4335?style=flat&logo=gmail)](mailto:singhyash0804@gmail.com)

---

## 🚀 Featured Primary Projects

### [🤖 AI Twin: Multi-Channel Copilot & Personal Knowledge Assistant](https://github.com/1yash0804/Ai_twin)
> *An agentic personal assistant platform featuring multi-channel ingestion, dual-tier memory management (Redis + Pinecone), and asynchronous document extraction.*

* **Dual-Tier Memory Architecture**:
  * **Short-Term Memory**: Redis-backed sliding window buffer storing the last 10 contextual interactions for zero-latency turn-by-turn chat recall.
  * **Long-Term Episodic Memory**: Semantic vector store powered by Pinecone and `all-MiniLM-L6-v2` embeddings (`langchain-huggingface`) with a **0.75 cosine similarity threshold** for precise episodic RAG retrieval.
* **Smart Intent Classification Engine**: Implemented rule-and-keyword intent routing separating prompts into `coding`, `factual`, and `personal memory recall` pipelines before hitting LLM inference.
* **Multi-Channel Message Ingestion**: Built a webhook gateway supporting real-time Telegram bot ingestion, normalizing multi-platform message payloads through strict data contracts.
* **Distributed Async Processing**: Celery task workers backed by Redis for offloading heavy document parsing, OCR, and embeddings extraction without blocking web request cycles.
* **Full-Stack Architecture**: Modern Next.js (App Router) dashboard with Tailwind CSS communicating with a high-performance FastAPI backend using SQLModel, JWT + OTP verification, and rate limiting.

```text
Stack: Python, FastAPI, Next.js (App Router), TypeScript, Pinecone, Redis, Celery, SQLModel, LangChain, HuggingFace
```

---

### [🚗 Autonomous UGV: Off-Road Semantic Segmentation](https://github.com/1yash0804/UGV_DualityHackthon)
> *Deep learning computer vision pipeline developed for an Unmanned Ground Vehicle (UGV) navigating extreme desert and off-road terrain.*

* **Multi-Class Terrain Segmentation**: Engineered an end-to-end semantic segmentation pipeline trained across **10 distinct off-road terrain classes** (sand, boulders, obstacles, traversable tracks, vegetation).
* **Deep Architecture & Augmentations**: Built on top of PyTorch and `segmentation_models_pytorch` with an extensive Albumentations pipeline (`HorizontalFlip`, `ShiftScaleRotate`, `Normalize`, `ToTensorV2`) to handle extreme contrast, dust interference, and sensor noise.
* **Benchmarking & Report Generation**: Automated inference evaluation tracking Mean Intersection over Union (mIoU) and pixel accuracy across validation batches, logging loss curves and generating visual performance reports (`generate_report.py`).
* **Edge Inference Optimization**: Designed lightweight PyTorch checkpointing (`best_model.pth`) for low-latency obstacle identification and traversability mapping on onboard edge GPUs.

```text
Stack: Python, PyTorch, segmentation_models_pytorch (smp), Albumentations, OpenCV, Pandas, CUDA
```

---

## 💡 Other Notable Projects

### [🚖 Cab_Ava: Availability Intelligence Layer (AIL)](https://github.com/1yash0804/Cab_Ava)
*Machine Learning, XGBoost, FastAPI, Node.js, Express*
* High-speed dynamic cab availability prediction microservice powered by an **XGBoost Classifier**.
* Evaluates real-time spatio-temporal features: `hour_of_day`, `drivers_nearby`, `local_demand_score`, `is_raining`, `lead_time_minutes`, and `trip_distance_km` to forecast booking availability and surge probabilities.

---

## 🛠️ Technical Skills

* **Languages**: Python, TypeScript, JavaScript, SQL, C++
* **AI, ML & Vision**: PyTorch, Semantic Segmentation, Transformers, LangChain, HuggingFace, Pinecone Vector DB, XGBoost, OpenCV, Albumentations
* **Backend & Systems**: FastAPI, Node.js, Express, Redis (Caching & Message Broker), Celery (Distributed Tasks), SQLModel, PostgreSQL, REST APIs
* **Frontend**: Next.js (App Router), React, Tailwind CSS, HTML5/CSS3
* **Tools & DevOps**: Git, GitHub, Docker, Linux, Kaggle GPU Environments
