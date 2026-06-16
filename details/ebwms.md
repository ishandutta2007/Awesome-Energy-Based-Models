# Energy-Based World Models (EBWMs)

Energy-Based World Models are used in Reinforcement Learning to model environment dynamics. They represent the compatibility between current states, actions, and future states using energy.

## Diagram
```mermaid
graph TD
    State[Current State s] --> EBWM
    Action[Action a] --> EBWM
    NextState[Proposed Next s'] --> EBWM
    EBWM --> Compatibility[Energy E]
    Compatibility -- Low Energy -- Plausible Transition
```

## Key Characteristics
- **Multi-modal Predictions**: Can represent multiple possible futures for the same action.
- **Planning**: Enables planning by minimizing energy over sequences of states.
- **Robotics**: Widely used for complex manipulation and navigation tasks.

[Back to README](../README.md)
