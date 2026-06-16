# Equilibrium Matching (EqM)

Equilibrium Matching (EqM) is a generative framework that learns a time-invariant equilibrium gradient of an implicit energy landscape. It avoids the sequential time-steps of diffusion models.

## Diagram
```mermaid
graph TD
    Noise[Starting Noise] --> Opt[Optimization Step]
    Opt --> Opt
    Opt --> Sample[Equilibrium Sample]
    subgraph Energy Surface
    Surface((Landscape))
    end
    Opt -- Gradient Descent -- Surface
```

## Key Characteristics
- **Implicit Energy**: Learns the gradient directly without an explicit energy function.
- **Time-Invariant**: No need for noise schedules or time conditioning.
- **Direct Optimization**: Samples are obtained via gradient descent at inference.

[Back to README](../README.md)
