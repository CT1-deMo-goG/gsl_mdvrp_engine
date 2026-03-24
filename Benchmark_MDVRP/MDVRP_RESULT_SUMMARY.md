# GSL Engine: MDVRP Result Summary
**Core Module:** `GSL_MDVRP_MASTER_V28`
**Optimization Strategy:** Deterministic Cluster-First, Route-Second (Zero-Tuning Policy)
**Execution Environment:** Mobile Architecture (Snapdragon, Android, Pydroid 3)

## 1. Extreme Large-Scale Stress Test (No Existing BKS)
This test evaluates the engine's capability to handle unprecedented logistical scale.

* **Instance:** `extreme_10k_benchmark.txt`
* **Network Size:** 10,000 Customers, 100 Depots
* **Total Distance (Cost):** 184,752.27
* **Fleet Deployed:** 1,371 Vehicles
* **Execution Time:** 8.908 seconds
* **Feasibility Status:** ✅ Fully Feasible (100% Demand Met, Capacity & Fleet Verified)

## 2. Standard Cordeau Benchmark Performance
Evaluated against the widely recognized Cordeau MDVRP datasets (p-series and pr-series). 

### Dataset: p-series (p01 - p23)
| Instance | GSL Cost | BKS Target | Gap (%) | Time (s) | Feasibility |
| :--- | :--- | :--- | :--- | :--- | :--- |
| p01 | 647.54 | 576.90 | +12.25% | 0.004s | ✅ Fully Feasible |
| p02 | 509.39 | 473.50 | +7.57% | 0.016s | ✅ Fully Feasible |
| p03 | 695.61 | 641.20 | +8.49% | 0.010s | ✅ Fully Feasible |
| p04 | 1088.78 | 1001.60 | +8.70% | 0.030s | ✅ Fully Feasible |
| p05 | 815.56 | 750.00 | +8.74% | 0.131s | ✅ Fully Feasible |
| p06 | 934.63 | 876.50 | +6.63% | 0.016s | ✅ Fully Feasible |
| p07 | 934.15 | 885.80 | +5.46% | 0.014s | ✅ Fully Feasible |
| p08 | 4556.46 | 4437.70 | +2.68% | 0.142s | ✅ Fully Feasible |
| p09 | 4135.37 | 3900.20 | +6.03% | 0.102s | ✅ Fully Feasible |
| p10 | 3956.61 | 3663.00 | +8.02% | 0.078s | ✅ Fully Feasible |
| p11 | 3824.64 | 3554.20 | +7.61% | 0.071s | ✅ Fully Feasible |
| p12 | 1365.69 | 1319.00 | +3.54% | 0.014s | ✅ Fully Feasible |
| p13 | 1365.69 | 1319.00 | +3.54% | 0.016s | ✅ Fully Feasible |
| p14 | 1365.69 | 1360.10 | +0.41% | 0.014s | ✅ Fully Feasible |
| p15 | 2731.37 | 2505.40 | +9.02% | 0.028s | ✅ Fully Feasible |
| p16 | 2731.37 | 2572.20 | +6.19% | 0.029s | ✅ Fully Feasible |
| p17 | 2731.37 | 2709.10 | +0.82% | 0.029s | ✅ Fully Feasible |
| p18 | 4097.06 | 3702.80 | +10.65% | 0.043s | ✅ Fully Feasible |
| p19 | 4097.06 | 3827.10 | +7.05% | 0.044s | ✅ Fully Feasible |
| p20 | 4097.06 | 4058.10 | +0.96% | 0.044s | ✅ Fully Feasible |
| p21 | 6145.58 | 5474.80 | +12.25% | 0.068s | ✅ Fully Feasible |
| p22 | 6145.58 | 5702.20 | +7.78% | 0.069s | ✅ Fully Feasible |
| p23 | 6145.58 | 6095.50 | +0.82% | 0.067s | ✅ Fully Feasible |

### Dataset: pr-series (pr01 - pr10)
| Instance | GSL Cost | BKS Target | Gap (%) | Time (s) | Feasibility |
| :--- | :--- | :--- | :--- | :--- | :--- |
| pr01 | 891.54 | 861.30 | +3.51% | 0.007s | ✅ Fully Feasible |
| pr02 | 1404.15 | 1307.60 | +7.38% | 0.028s | ✅ Fully Feasible |
| pr03 | 1905.90 | 1806.60 | +5.50% | 0.032s | ✅ Fully Feasible |
| pr04 | 2221.22 | 2072.50 | +7.17% | 0.075s | ✅ Fully Feasible |
| pr05 | 2549.65 | 2385.80 | +6.87% | 0.092s | ✅ Fully Feasible |
| pr06 | 2836.63 | 2723.30 | +4.16% | 0.138s | ✅ Fully Feasible |
| pr07 | 1184.62 | 1089.60 | +8.72% | 0.011s | ✅ Fully Feasible |
| pr08 | 1748.51 | 1666.60 | +4.91% | 0.031s | ✅ Fully Feasible |
| pr09 | 2323.79 | 2153.10 | +7.93% | 0.063s | ✅ Fully Feasible |
| pr10 | 3002.00 | 2921.80 | +2.74% | 0.106s | ✅ Fully Feasible |
