# Benchmark Methodology
**Module:** `GSL_MDVRP_MASTER_V28`

This document outlines the rigorous testing methodology applied to the GSL Engine to ensure performance transparency and reproducibility.

## 1. Execution Environment
Unlike traditional Operations Research (OR) benchmarks executed on high-performance servers, this engine is strictly validated under highly constrained hardware:
* **Hardware:** Mobile Device (Smartphone)
* **Processor:** Snapdragon Architecture
* **OS:** Android
* **Runtime:** Python via Pydroid 3
* **Validation Rationale:** Achieving sub-second processing on a mobile device proves the extreme efficiency and lightweight nature of the algorithmic core.

## 2. Zero-Tuning Policy
The most critical aspect of this benchmark is the strict adherence to a **Zero-Tuning Policy**.
* **Single Unified Script:** The exact same core algorithm was executed across all instances (from 50 nodes to 10,000 nodes).
* **No Instance-Specific Tweaking:** No hyperparameters were manually adjusted to fit specific datasets.
* **Autonomous Adaptation:** The engine mathematically adapts to customer distributions, depot counts, and capacities entirely on its own.

## 3. Dataset Categories
1. **Standard Academic Datasets (Cordeau):** Evaluated against p01-p23 and pr01-pr10. These establish the baseline comparison against global BKS (Best Known Solutions).
2. **Extreme Stress Test (10K Nodes):** A custom-generated 10,000-node, 100-depot dataset designed to push the engine to its absolute limits, proving linear scalability without memory overflow.

## 4. Verification Standards
Every output `.sol` file is subjected to deterministic verification:
* **Demand Validation:** 100% of customers must be served exactly once.
* **Capacity Constraint:** No vehicle load can exceed the strictly defined maximum capacity.
* **Fleet Constraint:** The total number of vehicles dispatched per depot must not exceed the specified limits.
