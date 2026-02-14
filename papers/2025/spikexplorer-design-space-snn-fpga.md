# SpikeExplorer: Hardware‑Oriented Design Space Exploration for Spiking Neural Networks on FPGA

**Authors:** Dario Padovano, Alessio Carpegna, Alessandro Savino, Stefano Di Carlo  
**Published:** May 2024  
**Venue:** *Electronics* (MDPI)  
**Link:** https://doi.org/10.3390/electronics13091744

## Problem Addressed
Designing efficient hardware accelerators for spiking neural networks (SNNs) on embedded systems — especially FPGAs — requires careful selection of network architectures, neuron models, and hardware parameters. Manual tuning across multiple objectives (accuracy, power, latency, area) is complex and time consuming, making it difficult for designers to reach optimal configurations.

## Key Idea
This paper introduces **SpikeExplorer**, a Python‑based design‑space exploration framework tailored for hardware‑oriented optimization of SNN accelerators targeting FPGAs. The tool supports **multi‑objective search** — including accuracy, area, latency, and power — and uses **Bayesian optimization** to automatically explore combinations of network configurations, neuron models, and hardware settings. This helps developers identify optimal trade‑offs for SNN deployment without needing manual trial‑and‑error. :contentReference[oaicite:1]{index=1}

## Hardware Perspective
- **Target Platform:** Digital FPGA accelerators  
- **Framework Features:**  
  - Modular and flexible design space exploration  
  - Multi‑objective optimization driven by hardware constraints  
  - Bayesian search strategy to balance competing goals (e.g., performance vs. energy)  
- **Outcomes:** Enables efficient mapping of SNN models onto hardware by tuning parameters automatically for specific design targets, making it suitable for edge or resource‑constrained systems. :contentReference[oaicite:2]{index=2}

## Results and Insights
Testing with benchmark tasks (e.g., MNIST classification) demonstrates that SpikeExplorer can achieve competitive performance while optimizing hardware metrics such as power consumption (~180 mW/image) and latency (~0.12 ms/image). The tool provides designers with the full set of explored design points and trade‑offs, offering clarity on how configuration changes impact hardware performance. :contentReference[oaicite:3]{index=3}

## Why This Paper Matters
This work matters because it automates the **hardware‑aware optimization** of SNN implementations — a core challenge in neuromorphic computing for embedded and edge applications. By combining design‑space exploration with FPGA optimization metrics, the framework helps researchers and engineers evaluate and generate efficient neuromorphic hardware designs **without deep manual tuning**. This supports rapid prototyping and informed decision‑making in SNN hardware research. :contentReference[oaicite:4]{index=4}

## References
- Padovano, D., Carpegna, A., Savino, A., & Di Carlo, S. (2024). *SpikeExplorer: Hardware‑Oriented Design Space Exploration for Spiking Neural Networks on FPGA*. *Electronics*, 13(9), 1744. https://doi.org/10.3390/electronics13091744
