# Diffusion Models (Score-Based EBMs)

Modern Diffusion Models, particularly Score-Based Generative Models, are closely linked to EBMs. They learn the "score function," which is the gradient of the log-density (the negative gradient of the energy).

## Diagram
```mermaid
graph LR
    Data --> Noise1[+Noise] --> Noise2[+Noise] --> Gaussian[Pure Noise]
    Gaussian --> Denoise1[-Noise] --> Denoise2[-Noise] --> Recovered[Clean Data]
    Denoise1 -- Score Function \nabla log p(x) -- Energy Landscape
```

## Key Characteristics
- **Score Matching**: Instead of the density, they model the gradient of the density.
- **Langevin Dynamics**: Used to sample from the model by following the score.
- **High Quality**: Currently state-of-the-art for image and video generation.

[Back to README](../README.md)
