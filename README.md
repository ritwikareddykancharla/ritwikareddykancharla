# Hi, I'm Ritwika — welcome to my research portfolio.  
<img src="assets/lottie/cat_big.gif" width="200px" align="right"/>

## 👩‍🔬 Research Scientist / Applied Scientist  
### Neural Optimization • Routing Foundation Models • Mechanistic Interpretability

My research focuses on **neural optimization for large-scale routing and supply-chain systems**. I work at the intersection of **mixed-integer programming (MILPs)**, **transformer architectures**, **diffusion priors**, and **world models**, with the goal of developing **Routing Foundation Models** that can reason, plan, and optimize complex networks with real-time inference.

Traditional routing pipelines rely on MILPs and heuristics that become brittle or intractable at Amazon scale. Meanwhile, modern neural networks exhibit emergent abilities in optimization, meta-learning, and planning. My work aims to unify these worlds: building **differentiable surrogate solvers** that approximate combinatorial reasoning, while retaining the structure and guarantees of classical optimization.

I am also deeply interested in **mechanistic interpretability**—understanding how neural routing models develop constraint circuits, represent flows, and perform multi-step refinement. Transparency is essential for high-stakes logistics systems, and my research emphasizes models that are both powerful and interpretable.


## 🔬 Research

### 📄 MILP-Transformer: A Neural Surrogate MILP Solver with Constraint Experts  
**Status:** Preprint (ICML 2026 submission)  
[📘 PDF](https://raw.githubusercontent.com/ritwikareddykancharla/neural-milp-surrogate/main/paper/main.pdf) ·  
[💻 Code](https://github.com/ritwikareddykancharla/neural-milp-surrogate)

A transformer-based neural surrogate for mixed-integer linear programs (MILPs), featuring:
- Constraint-specialized Mixture-of-Experts  
- Soft binary relaxations  
- Latent refinement loops  
- MILP-aware attention using primal–dual signals  
Achieves near-MILP quality with 50–100× faster inference on 50–200 node routing problems.

---

### 📄 Diffusion Priors for Routing Optimization (Working Title)  
**Status:** Draft manuscript · ICML 2026 submission  
[💻 Code (WIP)](https://github.com/ritwikareddykancharla/routing-diffusion)

Explores diffusion-based generative priors for producing feasible routing structures, enabling:
- Structure-aware denoising for binary routing decisions  
- Latent flow regularization  
- Multi-sample proposal generation for surrogate MILPs  

---

### 📄 Routing World Models for Multi-step Planning  
**Status:** Draft manuscript · ICML 2026 submission  
[💻 Code (WIP)](https://github.com/ritwikareddykancharla/routing-world-model)

A MuZero-style latent dynamics model for forecasting:
- congestion  
- future constraints  
- flow redistribution  
- multi-hop rollout effects  

Enables long-horizon planning on Amazon-style routing networks.

---

### 📚 RoutingAGI: Unified Architecture for Routing Optimization  
**Status:** Technical Monograph (100+ pages, in progress)  
A consolidated book-style document covering:
- MILP surrogates  
- routing diffusion  
- world models  
- constraint circuits  
- large-scale experiments  
- foundation models for optimization  

---

## 🚚 What I'm Working On — **RoutingAGI**

I'm building **RoutingAGI**, a spatial-transformer + SSM architecture designed for  
*Amazon-scale routing, spatial reasoning, and interpretable decision-making.*

RoutingAGI explores:

- 🗺️ Graph-based spatial encoding  
- 🌀 SSM/Mamba-style route planning  
- 🧩 Constraint-aware MoE (capacity, SLAs, time windows)  
- 📦 Multi-agent route generation  
- 🔍 Full mechanistic transparency (attention circuits, activations, geometry)

A routing model that not only performs…  
but **explains itself**.

---
