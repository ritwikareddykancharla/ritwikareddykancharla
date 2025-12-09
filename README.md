# Hi, I'm Ritwika — welcome to my research portfolio.  
<img src="assets/lottie/cat_big.gif" width="200px" align="right"/>

## 👩‍🔬 Research Scientist / Applied Scientist  
### Neural Optimization • Routing Foundation Models • Mechanistic Interpretability

My research focuses on **neural optimization for large-scale routing and supply-chain systems**. I work at the intersection of **mixed-integer programming (MILPs)**, **transformer architectures**, **diffusion priors**, and **world models**, with the goal of developing **Routing Foundation Models** that can reason, plan, and optimize complex networks with real-time inference.

Traditional routing pipelines rely on MILPs and heuristics that become brittle or intractable at Amazon scale. Meanwhile, modern neural networks exhibit emergent abilities in optimization, meta-learning, and planning. My work aims to unify these worlds: building **differentiable surrogate solvers** that approximate combinatorial reasoning, while retaining the structure and guarantees of classical optimization.

I am also deeply interested in **mechanistic interpretability**—understanding how neural routing models develop constraint circuits, represent flows, and perform multi-step refinement. Transparency is essential for high-stakes logistics systems, and my research emphasizes models that are both powerful and interpretable.

---

# Research

## 📄 **Routing Foundation Model (RFM): A Unified Neural Optimization Framework**  

[![PDF](https://img.shields.io/badge/PDF-RFM%20Monograph-red)](https://ritwikareddykancharla.github.io/rfm.pdf)
[![Code](https://img.shields.io/badge/Code-GitHub-2b3137?logo=github)](#)
[![Notebook](https://img.shields.io/badge/Colab-Notebook-yellow?logo=googlecolab)](#)

**Routing Foundation Model (RFM)** is my flagship research project:  
a **full-stack neural optimization architecture for routing MILPs**, designed for Amazon-scale networks.

RFM integrates **five modules** into a single differentiable system:

### **1. MILP-Aware Encoder**
A structured encoder that maps MILP components into embeddings:

- variable embeddings from cost coefficients + constraint participation  
- constraint embeddings capturing flow, capacity, timing, precedence  
- bipartite factor-graph representation of the constraint matrix \(A\)  
- dual/violation features that reflect MILP geometry  

This module grounds the network in **true MILP structure**, not just sequences.

---

### **2. MILP-Transformer (Surrogate Solver Core)**
A transformer stack that behaves like a **learned primal–dual solver**.

Key mechanisms:

- **Dual violation signals** \( v = \max(0, Ax - b) \)  
- **Dual ascent messages** \( A^\top v \)  
- **MILP-aware attention** that prioritizes constraint-heavy interactions  
- **Constraint-specialized Mixture-of-Experts**  
- **Latent refinement / proximal steps** pushing toward feasibility  

This module performs **iterative optimization-like refinement**, producing near-integral routing decisions in milliseconds.

---

### **3. Neural Routing Optimization Model (NROM)**
A global reasoning model combining:

- graph structure of the routing network  
- MILP encoder embeddings  
- multi-hop attention across facilities and arcs  

NROM constructs an **initial routing assignment** that is globally coherent before refinement.

---

### **4. Diffusion Routing Prior**
A diffusion model that learns the **distribution of feasible routing solutions**.

It enables:

- diverse feasible warm-starts for MILPs  
- feasibility-preserving denoising  
- multiple proposals for amortized optimization  
- robustness under disruptions (SLA spikes, congestion, outages)  

This dramatically reduces cold-start solver latency.

---

### **5. Routing World Model (SSM / Mamba)**
A sequential dynamics model that predicts:

- congestion propagation  
- delays and SLA risk  
- facility saturation  
- future constraint evolution  

Enables **lookahead planning**, MuZero-style rollouts, and dynamic routing policies.

---

### **RFM Summary**
RFM unifies:

- transformer-based surrogate solving  
- graph-structured MILP embeddings  
- diffusion generative priors  
- sequential world models  
- proximal refinement loops  

The result is a **differentiable optimization system** capable of generating fast, near-feasible routing decisions with strong generalization across network topologies.

Full monograph:  
**https://ritwikareddykancharla.github.io/rfm.pdf**

