# 03. Data Description, Understanding, Cleaning, and Transformation

## Data Description and Understanding

This section explains the main data used in the project and how it was prepared for simulation, financial analysis, and environmental evaluation.

The project data describes the physical production system, the simulation logic, and the financial assumptions of the proposed BioFuel waste tyre pyrolysis plant.

---

## General Production Data

| Parameter | Description | Value |
|---|---|---:|
| Average tyre weight | Assumed weight of one waste tyre | 10 kg |
| Tyres per day | Expected daily tyre input | 1000–1500 tyres |
| Daily production | Total daily material input | 10–15 tons/day |
| Pieces per tyre | Number of pieces after cutting | 4 pieces |
| Total pieces per day | Total pieces sent to shredding | 4000–6000 pieces |
| Reactor capacity | Maximum material per reactor batch | 10 tons |
| Reactor cycle time | Batch processing duration | 18–23 hours |

---

## Processing Time Assumptions

The simulation uses triangular distributions because industrial processing times can vary depending on machine condition, operator performance, tyre type, and material handling.

| Process | Processing Time | Unit | Capacity |
|---|---|---|---:|
| Debeading | Triangular(0.2, 0.3, 0.5) | minutes/tyre | 1 |
| Cutting | Triangular(0.15, 0.25, 0.4) | minutes/tyre | 1 |
| Shredding | Triangular(0.25, 0.4, 0.6) | minutes/piece | 1 |
| Reactor | Triangular(18, 20, 23) | hours/batch | 10 tons |

---

## Data Dictionary

| Field | Meaning | Why It Matters |
|---|---|---|
| `tyre_weight_kg` | Average weight of one tyre | Converts tyre count into tons |
| `tyres_per_day` | Number of tyres entering the system daily | Defines production load |
| `pieces_per_tyre` | Number of pieces after cutting | Determines shredding and batching load |
| `pieces_per_batch` | Number of pieces required for one batch | Controls reactor loading |
| `reactor_capacity_tons` | Reactor capacity per batch | Defines batch size |
| `reactor_cycle_time` | Time needed to process one batch | Determines system bottleneck |
| `capex` | Capital investment cost | Used in payback and ROI calculations |
| `opex` | Operating expenses | Affects net profit |
| `daily_profit` | Product profit per day | Used for feasibility results |

---

## Data Cleaning and Transformation

The raw assumptions were transformed into values suitable for the Simio simulation and economic model.

### 1. Tyre Count to Weight

```text
1000 tyres × 10 kg = 10,000 kg = 10 tons
1500 tyres × 10 kg = 15,000 kg = 15 tons
```

### 2. Tyres to Pieces

```text
1 tyre = 4 pieces
1000 tyres = 4000 pieces
1500 tyres = 6000 pieces
```

### 3. Reactor Batch Logic

```text
1 reactor batch = 10 tons
10 tons = 1000 tyres
1000 tyres = 4000 pieces
4000 pieces = 1 full reactor batch
```

### 4. Financial Scenario Preparation

The financial assumptions were organized into three scenarios:

| Scenario | Purpose |
|---|---|
| Conservative | Represents lower profit or higher risk conditions |
| Expected | Represents the most realistic project assumption |
| Optimistic | Represents better revenue or lower cost conditions |

---

## Key Performance Indicators

The simulation results are evaluated using the following KPIs:

| KPI | Purpose |
|---|---|
| Throughput | Measures system output |
| Reactor utilization | Shows how busy the reactor is |
| Machine utilization | Measures preprocessing equipment usage |
| Queue size | Identifies congestion |
| Waiting time | Measures delays before processing |
| Buffer level | Shows accumulation before batching |
| Completed batches | Shows production cycle achievement |
| Bottleneck location | Identifies the process limiting performance |

---

## Batching Logic

The pyrolysis reactor works in batch mode, so it cannot start until a full batch is ready. This is different from the preprocessing stages, which operate continuously.

The batching rule is:

```text
4000 tyre pieces = 1 full 10-ton reactor batch
```

This logic is important because it explains why material may wait in the buffer before entering the reactor.

---

## Simulation Understanding

The simulation shows the interaction between two types of processes:

1. **Continuous preprocessing**
   - Debeading
   - Cutting
   - Shredding

2. **Batch-based thermal processing**
   - Pyrolysis reactor

The difference between continuous flow and batch processing causes the reactor to become the main bottleneck.

---

## Main Data Insight

The key insight from the data is that the preprocessing stages are able to supply enough material, but the reactor controls the final output because it has a long batch cycle of 18–23 hours. Therefore, improving reactor performance would have the strongest impact on the whole system.
