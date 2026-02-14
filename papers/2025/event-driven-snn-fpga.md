# Spiking Neural Networks on FPGA: A Survey of Methodologies and Recent Advancements

**Authors:** Karamimanesh et al.
**Published:** 2025
**Venue:** Neural Networks (Elsevier)
**Link:** [https://doi.org/10.1016/j.neunet.2025.107256](https://doi.org/10.1016/j.neunet.2025.107256)

## Problem Addressed

Field-programmable gate arrays (FPGAs) are promising platforms for implementing spiking neural networks (SNNs), but there is no unified view of the different methods, trade-offs, and challenges involved in hardware implementations. Previous works mainly focus on software or theoretical models, leaving hardware designers with limited guidance for efficient FPGA-based SNN implementation.

## Key Idea

This paper reviews recent research on implementing and optimizing SNNs on FPGAs. It emphasizes leveraging parallel processing, event-driven computation, and sparse spike patterns to reduce latency and energy consumption compared with CPUs and GPUs. The authors categorize design techniques into input encoding, neuron implementation, learning rules, and system architecture, providing a comprehensive overview of how design choices impact performance and efficiency.

## Hardware Perspective

* **FPGA Suitability:** FPGAs offer high parallelism, reconfigurability, and low-latency computation, making them ideal for neuromorphic workloads.
* **Design Components:** Discussion includes spike encoding schemes, neuron circuit designs, learning rule integration, and system-level architecture.
* **Challenges:** Key challenges include integrating on-chip learning efficiently, scaling to larger networks, and handling sparse event-driven data effectively.

## Why This Paper Matters

This survey bridges the gap between neuromorphic algorithm research and hardware implementation, offering a roadmap for FPGA-based SNNs. It provides a clear understanding of current methodologies, highlights open research gaps, and offers practical insights for early-stage researchers interested in energy-efficient and hardware-aware SNN design.

## References

* Karamimanesh, A., et al. (2025). *Spiking Neural Networks on FPGA: A Survey of Methodologies and Recent Advancements*. Neural Networks, Elsevier. [https://doi.org/10.1016/j.neunet.2025.107256](https://doi.org/10.1016/j.neunet.2025.107256)
