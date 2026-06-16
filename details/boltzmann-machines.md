# Boltzmann Machines

Boltzmann Machines are stochastic recurrent neural networks that use a "Gibbs distribution" to model joint probability distributions. They are named after the Boltzmann distribution in statistical mechanics.

## Diagram
```mermaid
graph TD
    subgraph Visible Units
    V1((V1)) --- V2((V2))
    end
    subgraph Hidden Units
    H1((H1)) --- H2((H2))
    end
    V1 --- H1
    V1 --- H2
    V2 --- H1
    V2 --- H2
```

## Key Characteristics
- **Generative Model**: Can learn to represent and sample from complex data distributions.
- **Learning**: Typically uses Contrastive Divergence (CD) or simulated annealing.
- **Architecture**: Fully connected undirected graph with hidden and visible units.

[Back to README](../README.md)
