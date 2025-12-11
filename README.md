# Hi, I'm Ritwika — welcome to my research portfolio.  
<img src="assets/lottie/cat_big.gif" width="200px" align="right"/>

## 👩‍🔬 Research Scientist / Applied Scientist  
### Neural Optimization • Routing Models • Diffusion Priors • Mechanistic Interpretability

My research centers on **neural optimization for large-scale routing and supply-chain systems**, with a focus on designing architectures that can **reason, plan, and optimize** like classical solvers—while running at *neural-inference speed*. I work across **mixed-integer programming (MILPs)**, **transformer-based surrogate solvers**, **diffusion generative models**, and **state-space world models**, building toward a unified class of **Routing Foundation Models (RFMs)**.

Modern logistics networks—especially at Amazon scale—push traditional MILP solvers and heuristics to their limits. At the same time, contemporary neural networks are beginning to exhibit **emergent combinatorial reasoning**, iterative refinement behaviors, and powerful distributional priors. My work aims to bridge these worlds by developing **differentiable surrogate optimization frameworks** that blend:  
- the **algebraic structure** of MILPs,  
- the **expressiveness** of deep generative models, and  
- the **temporal forecasting ability** of world models.  

The goal is a new paradigm of **real-time, structure-aware routing intelligence** that generalizes across geography, demand, and network conditions.

I am also deeply interested in **mechanistic interpretability**—unpacking how neural routing models form constraint circuits, represent flows, propagate dual signals, and perform multi-step feasibility refinement. For high-stakes logistics systems, **transparent reasoning is not optional**, and interpretability is a first-class design principle in all my work.

---

# 🔬 Research

Below are my five research papers on neural routing and optimization.  
All implementations live in a unified repository:

🔗 **GitHub:** https://github.com/ritwikareddykancharla/diffusion-mamba-routing

---

## 📄 **1. Diffusion–Mamba Optimization for the Capacitated VRP (CVRP)**  
[![arXiv](https://img.shields.io/badge/arXiv-preprint-8B0000?logo=arxiv&logoColor=white)](#)
[![GitHub](https://img.shields.io/badge/Code-In%20Progress-yellow?logo=github)](https://github.com/ritwikareddykancharla/diffusion-mamba-routing)
[![Colab](https://img.shields.io/badge/Colab-demo-blue?logo=googlecolab)](#)

**Abstract —**  
This work introduces a diffusion-prior + Mamba refinement architecture for the Capacitated VRP.  
Our approach learns the geometry of feasible CVRP assignments and performs constraint-aware latent steps  
that mimic MILP optimization without search. The model serves as a neural surrogate solver capable  
of generating high-quality capacity-feasible routes with fast inference.

---

## 📄 **2. Temporal Diffusion Models for VRPTW**  
[![arXiv](https://img.shields.io/badge/arXiv-preprint-8B0000?logo=arxiv&logoColor=white)](#)
[![GitHub](https://img.shields.io/badge/Code-In%20Progress-yellow?logo=github)](https://github.com/ritwikareddykancharla/diffusion-mamba-routing)
[![Colab](https://img.shields.io/badge/Colab-demo-blue?logo=googlecolab)](#)

**Abstract —**  
We propose a time-conditioned diffusion model for VRPTW that incorporates  
window feasibility directly into the denoising dynamics.  
A lightweight Mamba temporal layer captures evolving slack and deadline structure,  
producing routes that remain consistent with service windows even under distribution shift.

---

## 📄 **3. Diffusion Optimization for Pickup–Delivery VRP (PDVRP)**  
[![arXiv](https://img.shields.io/badge/arXiv-preprint-8B0000?logo=arxiv&logoColor=white)](#)
[![GitHub](https://img.shields.io/badge/Code-In%20Progress-yellow?logo=github)](https://github.com/ritwikareddykancharla/diffusion-mamba-routing)
[![Colab](https://img.shields.io/badge/Colab-demo-blue?logo=googlecolab)](#)

**Abstract —**  
This paper extends diffusion-based routing to handle precedence, pairing,  
and pickup–delivery constraints. A structured latent representation ensures  
pickup and delivery nodes remain linked throughout the denoising trajectory,  
while Mamba refinement enforces feasibility with respect to precedence  
and vehicle capacity constraints.

---

## 📄 **4. Diffusion–Mamba Models for Multi-Depot VRP (MDVRP)**  
[![arXiv](https://img.shields.io/badge/arXiv-preprint-8B0000?logo=arxiv&logoColor=white)](#)
[![GitHub](https://img.shields.io/badge/Code-In%20Progress-yellow?logo=github)](https://github.com/ritwikareddykancharla/diffusion-mamba-routing)
[![Colab](https://img.shields.io/badge/Colab-demo-blue?logo=googlecolab)](#)

**Abstract —**  
We develop depot-aware diffusion routes jointly with a Mamba global refinement  
process that assigns customers to depots while respecting heterogeneous fleets  
and capacity. The model captures cross-depot coupling and produces coherent  
multi-region routing plans with a single forward pass.

---

## 📄 **5. Online Diffusion Routing for Dynamic VRP (DVRP)**  
[![arXiv](https://img.shields.io/badge/arXiv-preprint-8B0000?logo=arxiv&logoColor=white)](#)
[![GitHub](https://img.shields.io/badge/Code-In%20Progress-yellow?logo=github)](https://github.com/ritwikareddykancharla/diffusion-mamba-routing)
[![Colab](https://img.shields.io/badge/Colab-demo-blue?logo=googlecolab)](#)

**Abstract —**  
This work introduces an online routing framework that performs  
diffusion rollouts over short-horizon futures, guided by a Mamba world model  
capturing traffic and request dynamics. The method enables anticipatory routing  
under real-time constraints and dynamic customer arrivals.

---

**All five works share a common philosophy:**  
*Diffusion provides the structural prior; Mamba provides the optimization refinement.*  



