

This document highlights key architectural differences between
**Intel Loihi** and **IBM TrueNorth**, focusing on hardware design
choices and system-level trade-offs in neuromorphic processors.

---

## Key Architectural Insights

- **Event-Driven Philosophy (Both Systems)**  
  Both Loihi and TrueNorth process information using spike-based,
  event-driven computation, avoiding continuous clock-driven execution
  typical of conventional CPUs and GPUs.

- **Programmability vs Fixed-Function Design**  
  Loihi supports programmable neuron models and on-chip learning,
  making it suitable for research and algorithm exploration.
  TrueNorth uses fixed neuron and synapse models to maximize
  energy efficiency and scalability.

- **Learning Support**  
  Loihi includes dedicated hardware mechanisms for synaptic plasticity,
  enabling local learning rules.
  TrueNorth relies on offline training, simplifying hardware
  but limiting adaptability.

- **Interconnect and Communication**  
  Loihi employs an asynchronous network-on-chip optimized for sparse
  spike traffic.
  TrueNorth uses a deterministic routing fabric within a globally
  clocked system, trading flexibility for predictability.

- **Power Efficiency Trade-offs**  
  TrueNorth achieves extremely low power consumption through rigid
  architectural constraints.
  Loihi consumes slightly more power but gains flexibility and
  learning capability.

- **Target Use Cases**  
  Loihi is oriented toward neuromorphic research, prototyping,
  and adaptive systems.
  TrueNorth is designed for large-scale deployment where energy
  efficiency and reliability are paramount.

---

## Design Takeaway

These architectures demonstrate that neuromorphic efficiency
is achieved not through biological realism, but through
**sparse computation, event-driven communication, and
carefully constrained hardware design**.
