# Joint Energy-Based Models (JEMs)

Joint Energy-Based Models (JEMs) reinterpret standard discriminative classifiers (like a ResNet with Softmax) as Energy-Based Models. This allows a single model to perform classification, generation, and OOD detection simultaneously.

## Diagram
```mermaid
graph LR
    Input --> Backbone[Neural Network]
    Backbone --> Logits[Logits f_y]
    Logits --> Classifier[Softmax P(y|x)]
    Logits --> EBM[Energy E(x) = -log \sum exp f_y]
```

## Key Characteristics
- **Dual Use**: Works as both a classifier and a generative model.
- **OOD Detection**: Energy scores can effectively identify out-of-distribution data.
- **Minimal Changes**: Requires no architectural changes to existing classifiers.

[Back to README](../README.md)
