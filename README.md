# Awesome-Energy-Based-Models
## Energy-Based Models (EBMs)

Energy-Based Models (EBMs) assign low energy to valid or likely data points and high energy to invalid ones. They function like a mathematical landscape where valid data sits in "valleys" and incorrect data forms "hills". By doing this, they avoid calculating complex probability distributions while still modeling complex relationships.

---

## Key Types & Examples of EBMs

### 1. Foundational & Probabilistic EBMs
| Model | Description | Year | Original Paper |
| :--- | :--- | :--- | :--- |
| **Hopfield Networks** | The simplest form of an EBM, acting as a recurrent neural network that serves as an associative memory system. The energy function calculates how close a network state is to a stored memory, allowing it to reconstruct noisy inputs. | 1982 | [Neural networks and physical systems with emergent collective computational abilities](https://www.pnas.org/doi/10.1073/pnas.79.8.2554) |
| **Boltzmann Machines** | Fully connected, undirected graphical models. They model joint probability distributions using a "Gibbs distribution", where states of the network have an energy corresponding to their thermodynamic probability. | 1985 | [A learning algorithm for Boltzmann machines](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1551-6708.1985.tb00120.x) |
| **Restricted Boltzmann Machines (RBMs)** | A highly restricted, bipartite version of the Boltzmann machine. By preventing connections within the same layer, RBMs become much easier to train and serve as fundamental building blocks for historical "Deep Belief Networks". | 1986 | [Information processing in dynamical systems: Foundations of harmony theory](https://dl.acm.org/doi/10.5555/104279.104290) |

### 2. Deep & Hybrid EBM Architectures
| Model | Description | Year | Original Paper |
| :--- | :--- | :--- | :--- |
| **Deep Energy-Based Models** | EBMs where the energy function is parameterized by a deep neural network (e.g., a Convolutional Neural Network). These models can learn implicit features of raw data without needing to define explicit probabilistic rules, often leveraging techniques like **Contrastive Divergence** to lower the energy of real data while raising the energy of generated ones. | 2011 | [Learning Deep Energy Models](https://icml.cc/2011/papers/538_icmlpaper.pdf) |
| **Joint Energy-Based Models (JEMs)** | These models reframe standard classifiers (like ResNets with softmax outputs) to act as EBMs without requiring structural changes to the neural network. By interpreting logits as unnormalized negative energies, JEMs allow a standard classifier to naturally perform data generation, out-of-distribution detection, and classification simultaneously. | 2019 | [Your Classifier is Secretly an Energy Based Model and You Should Treat it Like One](https://arxiv.org/abs/1912.03263) |

### 3. Modern Generative & Implicit EBM Approaches
| Model | Description | Year | Original Paper |
| :--- | :--- | :--- | :--- |
| **Diffusion Models** | While typically viewed as separate, many modern **Diffusion Models** (like Score-Based Generative Models) share a direct mathematical lineage with EBMs. They learn to estimate the gradient of the log-density of the data (also called the score), essentially navigating an energy landscape to denoise and generate images. | 2015 | [Deep Unsupervised Learning using Equilibrium Thermodynamics](https://arxiv.org/abs/1503.03585) |
| **Equilibrium Matching (EqM)** | A generative framework that learns the equilibrium gradient of an implicit energy landscape. Instead of sequential time-stepping like diffusion, EqMs utilize direct optimization at inference time to obtain samples through gradient descent on the learned energy surface. | 2025 | [Equilibrium Matching: Generative Modeling with Implicit Energy-Based Models](https://arxiv.org/abs/2510.00752) |
| **Energy-Based World Models (EBWMs)** | Used heavily in advanced reinforcement learning and robotics, these models shape energy landscapes to anticipate how an environment will react. They can efficiently handle multi-modal predictions, representing all possible future outcomes by minimizing the energy for plausible states. | 2019 | [Model-Based Planning with Energy-Based Models](https://arxiv.org/abs/1909.06878) |
