# Mapping Neuromorphic Hardware Concepts to Loihi and TrueNorth

This document connects fundamental neuromorphic hardware concepts
to real-world implementations such as **Intel Loihi** and **IBM TrueNorth**.

The goal is to understand how abstract neuromorphic principles
are realized in practical silicon architectures.

---

## 1. Event-Driven Computation

### Hardware Concept
- Asynchronous spike-based communication
- No global clock
- Computation triggered by neural events

### Loihi
- Fully asynchronous spike routing
- Event-driven neuron updates
- Reduced idle power consumption

### TrueNorth
- Globally clocked but functionally event-driven
- Spikes encoded as binary events
- Optimized for sparse neural activity

**Hardware Insight:**  
Event-driven designs significantly reduce power by avoiding continuous switching.

---

## 2. Neuron Implementation

### Hardware Concept
- Integrate-and-fire neuron models
- Threshold-based spike generation

### Loihi
- Programmable neuron models
- Supports on-chip learning and plasticity

### TrueNorth
- Fixed neuron model
- Highly optimized digital implementation

**Trade-off:**  
Programmability vs energy efficiency.

---

## 3. Synaptic Connectivity

### Hardware Concept
- Large-scale synaptic fan-in/fan-out
- Sparse connectivity

### Loihi
- Flexible synaptic routing
- Supports learning rules

### TrueNorth
- Fixed synaptic weights
- Massive parallelism with constrained routing

**Hardware Insight:**  
Routing efficiency is as important as neuron computation.

---

## 4. Digital vs Mixed-Signal Design

| Aspect | Loihi | TrueNorth |
|------|-------|-----------|
| Design style | Digital / mixed | Fully digital |
| Learning | On-chip | Offline |
| Flexibility | High | Fixed |
| Power efficiency | High | Extremely high |

---

## 5. Architectural Lessons

- Neuromorphic efficiency comes from **sparsity**
- Event-based interconnects dominate performance
- Learning support increases hardware complexity
- Fixed-function designs maximize energy efficiency

---

## Conclusion

Loihi and TrueNorth demonstrate two valid hardware strategies
for neuromorphic computing:

- **Loihi:** Research flexibility and learning
- **TrueNorth:** Large-scale efficiency and deployment

Understanding these systems provides valuable insight
for future neuromorphic hardware design.
