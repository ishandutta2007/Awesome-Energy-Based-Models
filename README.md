<div align="center">

# ⚡ Awesome Energy-Based Models (EBMs) ⚡

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/ishandutta2007/Awesome-Energy-Based-Models/graphs/commit-activity)
<a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

**A curated list of awesome Energy-Based Models, research papers, and resources.**

![EBM Banner](https://capsule-render.vercel.app/render?type=soft&color=auto&height=300&section=header&text=Energy-Based%20Models&fontSize=90)

---

<p align="center">
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHJ4ZGZ6eXlyeXlyeXlyeXlyeXlyeXlyeXlyeXlyeXlyeXlyeXlyJmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/3o7TKMGpxx6rQeWtkc/giphy.gif" width="400" />
</p>

</div>

## 🌌 Introduction to Energy-Based Models (EBMs)

Energy-Based Models (EBMs) assign low energy to valid or likely data points and high energy to invalid ones. They function like a mathematical landscape where valid data sits in **"valleys"** and incorrect data forms **"hills"**. By doing this, they avoid calculating complex probability distributions while still modeling complex relationships.

---

## 🚀 Key Types & Examples of EBMs

### 1. 🧱 Foundational & Probabilistic EBMs
| Model | Description | Year | Original Paper | More Info |
| :--- | :--- | :--- | :--- | :--- |
| **Hopfield Networks** | The simplest form of an EBM, acting as a recurrent neural network that serves as an associative memory system. | 1982 | [Paper](https://www.pnas.org/doi/10.1073/pnas.79.8.2554) | [Detail Page](./details/hopfield-networks.md) |
| **Boltzmann Machines** | Fully connected, undirected graphical models. They model joint probability distributions using a "Gibbs distribution". | 1985 | [Paper](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1551-6708.1985.tb00120.x) | [Detail Page](./details/boltzmann-machines.md) |
| **Restricted Boltzmann Machines (RBMs)** | A highly restricted, bipartite version of the Boltzmann machine. fundamental building blocks for DBNs. | 1986 | [Paper](https://dl.acm.org/doi/10.5555/104279.104290) | [Detail Page](./details/rbms.md) |

### 2. 🧠 Deep & Hybrid EBM Architectures
| Model | Description | Year | Original Paper | More Info |
| :--- | :--- | :--- | :--- | :--- |
| **Deep Energy-Based Models** | EBMs where the energy function is parameterized by a deep neural network (e.g., a CNN). | 2011 | [Paper](https://icml.cc/2011/papers/538_icmlpaper.pdf) | [Detail Page](./details/deep-ebms.md) |
| **Joint Energy-Based Models (JEMs)** | Models that reframe standard classifiers (like ResNets) to act as EBMs without structural changes. | 2019 | [Paper](https://arxiv.org/abs/1912.03263) | [Detail Page](./details/jems.md) |

### 3. 🌀 Modern Generative & Implicit EBM Approaches
| Model | Description | Year | Original Paper | More Info |
| :--- | :--- | :--- | :--- | :--- |
| **Diffusion Models** | Share a direct mathematical lineage with EBMs. They learn to estimate the gradient of the log-density. | 2015 | [Paper](https://arxiv.org/abs/1503.03585) | [Detail Page](./details/diffusion-models.md) |
| **Equilibrium Matching (EqM)** | A generative framework that learns the equilibrium gradient of an implicit energy landscape. | 2025 | [Paper](https://arxiv.org/abs/2510.00752) | [Detail Page](./details/eqm.md) |
| **Energy-Based World Models (EBWMs)** | Shape energy landscapes to anticipate environment reactions in RL and robotics. | 2019 | [Paper](https://arxiv.org/abs/1909.06878) | [Detail Page](./details/ebwms.md) |

## 📈 Star History
<div align="center">
   <a href="https://www.star-history.com/#ishandutta2007/Awesome-Energy-Based-Models&Date">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=ishandutta2007/Awesome-Energy-Based-Models&type=Date&theme=dark" />
      <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=ishandutta2007/Awesome-Energy-Based-Models&type=Date" />
      <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=ishandutta2007/Awesome-Energy-Based-Models&type=Date" />
    </picture>
   </a>
</div>


