# Restricted Boltzmann Machines (RBMs)

Restricted Boltzmann Machines are a variant of Boltzmann Machines with the restriction that there are no connections between units in the same layer. This bipartite structure makes training significantly more efficient.

## Diagram
```mermaid
graph LR
    subgraph Visible
    V1((V1))
    V2((V2))
    V3((V3))
    end
    subgraph Hidden
    H1((H1))
    H2((H2))
    end
    V1 --- H1
    V1 --- H2
    V2 --- H1
    V2 --- H2
    V3 --- H1
    V3 --- H2
```

## Key Characteristics
- **Bipartite Graph**: No intra-layer connections.
- **Deep Belief Networks**: RBMs are the building blocks of DBNs.
- **Efficiency**: Can be trained using the Contrastive Divergence (CD) algorithm.

[Back to README](../README.md)
