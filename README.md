# Awesome-Energy-Based-Models
## Energy-Based Models (EBMs)

Energy-Based Models (EBMs) assign low energy to valid or likely data points and high energy to invalid ones. They function like a mathematical landscape where valid data sits in "valleys" and incorrect data forms "hills". By doing this, they avoid calculating complex probability distributions while still modeling complex relationships.

---

## Key Types & Examples of EBMs

### 1. Foundational & Probabilistic EBMs
* **Hopfield Networks**: The simplest form of an EBM, acting as a recurrent neural network that serves as an associative memory system. The energy function calculates how close a network state is to a stored memory, allowing it to reconstruct noisy inputs.
* **Boltzmann Machines**: Fully connected, undirected graphical models. They model joint probability distributions using a "Gibbs distribution", where states of the network have an energy corresponding to their thermodynamic probability.
* **Restricted Boltzmann Machines (RBMs)**: A highly restricted, bipartite version of the Boltzmann machine. By preventing connections within the same layer, RBMs become much easier to train and serve as fundamental building blocks for historical "Deep Belief Networks".

### 2. Deep & Hybrid EBM Architectures
* **Deep Energy-Based Models**: EBMs where the energy function is parameterized by a deep neural network (e.g., a Convolutional Neural Network). These models can learn implicit features of raw data without needing to define explicit probabilistic rules, often leveraging techniques like **Contrastive Divergence** to lower the energy of real data while raising the energy of generated ones.
* **Joint Energy-Based Models (JEMs)**: These models reframe standard classifiers (like ResNets with softmax outputs) to act as EBMs without requiring structural changes to the neural network. By interpreting logits as unnormalized negative energies, JEMs allow a standard classifier to naturally perform data generation, out-of-distribution detection, and classification simultaneously. 

### 3. Modern Generative & Implicit EBM Approaches
* **Diffusion Models**: While typically viewed as separate, many modern **Diffusion Models** (like Score-Based Generative Models) share a direct mathematical lineage with EBMs. They learn to estimate the gradient of the log-density of the data (also called the score), essentially navigating an energy landscape to denoise and generate images.
* **Equilibrium Matching (EqM)**: A generative framework that learns the equilibrium gradient of an implicit energy landscape. Instead of sequential time-stepping like diffusion, EqMs utilize direct optimization at inference time to obtain samples through gradient descent on the learned energy surface. 
* **Energy-Based World Models (EBWMs)**: Used heavily in advanced reinforcement learning and robotics, these models shape energy landscapes to anticipate how an environment will react. They can efficiently handle multi-modal predictions, representing all possible future outcomes by minimizing the energy for plausible states.
