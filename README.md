# Hi, I’m Ritwika — welcome to my applied ML systems portfolio  
<img src="assets/lottie/cat_big.gif" width="200px" align="right"/>

## 👩‍🔬 Applied Scientist 
### End-to-End ML Systems • Retrieval • Computer Vision • LLM Serving

I build **end-to-end machine learning systems** that integrate modern models with
production-style infrastructure, evaluation, and deployment constraints.

My work focuses on **applied ML pipelines** rather than isolated models — spanning
information retrieval, multimodal learning, computer vision, and low-latency LLM
serving. Each project mirrors how ML systems are designed, debugged, and scaled
in real-world environments.

---

## 📌 Selected Applied ML Systems

---

### 1️⃣ Hybrid Retrieval-Augmented Question Answering Pipeline   [![GitHub](https://img.shields.io/badge/GitHub-black?logo=github)](https://github.com/ritwikareddykancharla/hybrid-rag-qa)  
**LLMs · Information Retrieval · RAG**

An end-to-end **retrieval-augmented QA system** over heterogeneous data sources,
including structured tables and unstructured documents.

- Hybrid sparse–dense retrieval using **BM25 (OpenSearch)** and **dense embeddings**
- **Cross-encoder reranking** to improve top-k precision
- **Grounded generation with explicit source attribution**
- Offline evaluation via **retrieval recall** and **answer faithfulness**

This system treats RAG as a **controlled, auditable pipeline**, not a black-box LLM.

---

### 2️⃣ Real-Time Video Object Detection and Tracking Pipeline   [![GitHub](https://img.shields.io/badge/GitHub-black?logo=github)](https://github.com/ritwikareddykancharla/multi-object-tracking-pipeline)  
**Computer Vision · Deep Learning Systems**

A real-time video analytics pipeline implementing **tracking-by-detection**
for persistent multi-object tracking under latency constraints.

- Object detection using **YOLOv8**
- Multi-object tracking via **ByteTrack / DeepSORT**
- GPU-accelerated inference with **structured outputs (CSV / JSON)**
- Evaluation using **IDF1** and **MOTA**, with failure analysis

Designed to produce stable object identities across video sequences.

---

### 3️⃣ Multimodal Product Representation and Retrieval Pipeline  [![GitHub](https://img.shields.io/badge/GitHub-black?logo=github)](https://github.com/ritwikareddykancharla/multimodal-product-retrieval)  
**Vision–Language Models · Multimodal Retrieval**

A **joint vision–language embedding system** enabling cross-modal retrieval
between product images and textual descriptions.

- CLIP-style joint embeddings for images and text
- Approximate nearest neighbor search using **FAISS**
- Image↔text retrieval via cosine similarity
- Evaluation using **Recall@K** and embedding alignment analysis

Structured for scalability to large product catalogs.

---

### 4️⃣ Low-Latency Large Language Model Inference Benchmark  [![GitHub](https://img.shields.io/badge/GitHub-black?logo=github)](https://github.com/ritwikareddykancharla/llm-inference-benchmark)  
**ML Systems · LLM Serving**

A benchmarking framework for **production-style LLM serving**, focused on
latency–throughput tradeoffs under realistic request workloads.

- Serving backends using **vLLM** and **SGLang**
- Evaluation of **dynamic batching**, **KV-cache reuse**, and concurrency
- Measurement of **P50 / P95 latency** and throughput saturation
- Analysis of system-level scalability bottlenecks

This project emphasizes **systems-level reasoning** over model internals.

---

## 📐 Design Philosophy

Across all projects, I prioritize:

- Explicit separation of system components  
- Industry-standard open-source tooling  
- Evaluation-driven iteration and failure analysis  
- Transparency over black-box behavior  
- Production-oriented architectural tradeoffs  

Each system is intentionally scoped to be **interview-defensible** and
representative of real-world ML deployments.

---

## 📊 Notes

This portfolio is curated to showcase applied ML system design rather than
research novelty alone. All repositories are independently runnable,
documented, and designed for technical discussion.
