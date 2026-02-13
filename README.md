# Hi, I’m Ritwika — Software Engineer for AI Infrastructure 🛡️🤖
<img src="assets/lottie/cat_big.gif" width="200px" align="right"/>

🛠️ I build **high-reliability infrastructure** for AI systems, focusing on the hardest engineering challenges: **low-latency media transport**, **inference observability**, **distributed storage**, and **structured reasoning pipelines**.

My work sits at the intersection of **Site Reliability Engineering (SRE)** and **ML Systems**. I prioritize observability over black-box monitoring, correctness over convenience, and performance over abstraction.

These projects demonstrate specific skills for scaling AI:
- **Reliability:** Monitoring the "token path" and GPU behavior.
- **Networking:** Building real-time media infrastructure (WebRTC/SFU).
- **Storage:** Engineering database internals from scratch.
- **Data:** Structuring knowledge for complex reasoning.

---

## 🧪 Recent Systems Projects

---

### 🕸️ [graph-enhanced-rag](https://github.com/ritwikareddykancharla/graph-enhanced-rag)  
**Knowledge Graph Construction Engine (Knowledge Innovation)**

Standard RAG struggles with multi-hop reasoning. This backend system ingests unstructured documents and autonomously builds a **Knowledge Graph** inside Postgres to capture relationships between entities.

- **Extraction:** Uses an LLM to extract entities and relations (`Server A` → *depends_on* → `Database B`) from raw text.
- **Storage:** Utilizes **Recursive CTEs** in Postgres to traverse the graph efficiently without a separate graph DB.
- **Querying:** An API that answers questions like "If Node X goes down, what features are impacted?" by traversing the graph structure.

**Tech Stack:** `Python (FastAPI)` `Postgres` `Recursive CTEs` `Pydantic`

---

### 📡 [token-path-observability](https://github.com/ritwikareddykancharla/token-path-observability)  
**Observability stack for LLM inference (AI Reliability)**

Standard web metrics (CPU/RAM) fail for LLMs. This project provides a dedicated monitoring dashboard for the **"token path"**—the lifecycle of a prompt from request to final token generation.

- **Metrics:** Tracks **Time-to-First-Token (TTFT)** and **Inter-Token Latency (ITL)** to diagnose user-perceived lag.
- **Accelerator Awareness:** Monitors GPU VRAM vs. Compute utilization to identify memory-bound bottlenecks.
- **Implementation:** Prometheus exporters for `vLLM`/`TGI`, custom Grafana dashboards.
- **Impact:** Enables proactive detection of "tail latencies" in model serving.

**Tech Stack:** `Python` `Prometheus` `Grafana` `Docker` `NVIDIA SMI`

---

### 🖥️ [realtime-sfu-engine](https://github.com/ritwikareddykancharla/realtime-sfu-engine)  
**Custom Selective Forwarding Unit in Go (Realtime WebRTC)**

Most engineers use black-box SDKs (Twilio/Agora). I built the core media server infrastructure from scratch to understand how to move audio/video data instantly.

- **Core Logic:** Built a minimalist **Selective Forwarding Unit (SFU)** using the Pion WebRTC library. It routes video streams between users *without* decoding them (preserving CPU).
- **Adaptive Streaming:** Implemented **Simulcast** routing—the server detects if a user's network slows down and automatically switches them to a lower-resolution stream.
- **Signaling:** Custom WebSocket signaling server for SDP offer/answer exchange.

**Tech Stack:** `Go` `Pion WebRTC` `WebSockets` `Docker`

---

### 🌳 [lsm-storage-engine](https://github.com/ritwikareddykancharla/lsm-storage-engine)  
**Custom Key-Value Store with LSM Tree (Online Storage)**

To understand how databases scale, I built one. This is a from-scratch implementation of a Log-Structured Merge-tree (LSM), the architecture used by RocksDB and Cassandra.

- **Write Path:** Implements an in-memory **MemTable** (Skip List) and persistent **SSTables** for high-throughput writes.
- **Crash Recovery:** Implements a **Write-Ahead Log (WAL)** to ensure durability during failures.
- **Read Optimization:** Implements **Bloom Filters** to reduce disk I/O for non-existent keys.
- **Compaction:** Background process merging SSTables to reclaim space and speed up reads.

**Tech Stack:** `C++` (or `Rust`) `Posix Threads` `File I/O`

---

## 📌 Notes

This portfolio is focused on **systems fundamentals**.  
Each project targets a specific bottleneck in modern AI companies: inference latency, media transport, data durability, and knowledge structure.
