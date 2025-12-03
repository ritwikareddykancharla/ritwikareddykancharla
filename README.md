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

[![arXiv](https://img.shields.io/badge/arXiv-Preprint%20-b31b1b.svg)](#)
[![PDF](https://img.shields.io/badge/PDF-Main%20Paper-blue)](https://raw.githubusercontent.com/ritwikareddykancharla/neural-milp-surrogate/main/paper/main.pdf)
[![Code](https://img.shields.io/badge/Code-GitHub-2b3137?logo=github)](https://github.com/ritwikareddykancharla/neural-milp-surrogate)
[![Colab](https://img.shields.io/badge/Colab-Open%20Notebook-yellow?logo=googlecolab)](https://colab.research.google.com/github/ritwikareddykancharla/neural-milp-surrogate/blob/main/notebooks/00_setup.ipynb)


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

## 🔬 Research

---

### 📄 MILP-Transformer: A Neural Surrogate MILP Solver with Constraint Experts  
**Status:** Preprint (ICML 2026 submission)

[![arXiv](https://img.shields.io/badge/arXiv-Preprint%20(coming%20soon)-b31b1b.svg)](#)
[![PDF](https://img.shields.io/badge/PDF-Main%20Paper-blue)](https://raw.githubusercontent.com/ritwikareddykanclarla/neural-milp-surrogate/main/paper/main.pdf)
[![Code](https://img.shields.io/badge/Code-GitHub-2b3137?logo=github)](https://github.com/ritwikareddykancharla/neural-milp-surrogate)
[![Colab](https://img.shields.io/badge/Colab-Notebook-yellow?logo=googlecolab)](https://colab.research.google.com/github/ritwikareddykancharla/neural-milp-surrogate/blob/main/notebooks/00_setup.ipynb)

**Abstract:**  
A transformer-based neural surrogate for mixed-integer linear programs (MILPs).  
The model integrates MILP algebra into attention using constraint violations and dual-like signals,  
introduces constraint-specialized Mixture-of-Experts, and performs latent refinement steps that  
approximate optimization. Achieves near-MILP feasibility and 50–100× faster inference on  
50–200 node routing problems.

---

### 📄 Diffusion Priors for Routing Optimization (Working Title)
**Status:** Draft manuscript · ICML 2026 submission 

[![arXiv](https://img.shields.io/badge/arXiv-Preprint%20(coming%20soon)-b31b1b.svg)](#)
[![Code](https://img.shields.io/badge/Code-GitHub-2b3137?logo=github)](https://github.com/ritwikareddykancharla/routing-diffusion)
[![Colab](https://img.shields.io/badge/Colab-Notebook-yellow?logo=googlecolab)](https://colab.research.google.com/github/ritwikareddykancharla/routing-diffusion/blob/main/notebooks/00_setup.ipynb)

**Abstract:**  
Explores diffusion-based generative priors for routing and flow optimization.  
The diffusion process learns the geometry of feasible routing structures and performs  
structure-aware denoising aligned with MILP constraints. Enables diverse route sampling,  
feasibility restoration, and multi-sample proposal generation for surrogate MILP solvers.

---

### 📄 Routing World Models for Multi-step Planning (Working Title)
**Status:** Draft manuscript · ICML 2026 submission

[![arXiv](https://img.shields.io/badge/arXiv-Preprint%20(coming%20soon)-b31b1b.svg)](#)
[![Code](https://img.shields.io/badge/Code-GitHub-2b3137?logo=github)](https://github.com/ritwikareddykancharla/routing-world-model)
[![Colab](https://img.shields.io/badge/Colab-Notebook-yellow?logo=googlecolab)](https://colab.research.google.com/github/ritwikareddykancharla/routing-world-model/blob/main/notebooks/00_setup.ipynb)

**Abstract:**  
A MuZero-inspired routing world model that predicts congestion, flow propagation,  
constraint evolution, and multi-step rollout effects. The latent dynamics model enables  
long-horizon planning on Amazon-style routing networks and supports differentiable internal  
lookahead for optimization-aware decision-making.

---


