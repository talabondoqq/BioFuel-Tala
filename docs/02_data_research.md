# 02. Data Research and Acquiring Effort

## Purpose of Data Collection

The purpose of data collection was to gather the information required to build the simulation model, evaluate financial feasibility, estimate environmental impact, and design the digital monitoring prototype.

The project required different types of data, including production assumptions, processing times, reactor capacity, product output assumptions, investment costs, operating costs, revenue estimates, and monitoring requirements.

---

## Data Sources

The project data was collected and estimated from several sources:

| Source | Data Used | Purpose |
|---|---|---|
| BioFuel Company project assumptions | Production capacity, process flow, system concept | To represent the proposed plant structure |
| Literature review | Waste tyre pyrolysis outputs, process behavior, environmental context | To support technical and environmental assumptions |
| Simulation modeling requirements | Processing times, capacities, queues, batching logic | To build the Simio model |
| Economic estimates | CAPEX, OPEX, revenue, profit scenarios | To evaluate financial feasibility |
| Environmental assumptions | Product recovery and waste reduction logic | To evaluate sustainability contribution |
| Digital monitoring prototype requirements | Dashboard screens, alerts, reports, reactor status | To support the app concept |

---

## Main Data Collected

The main data collected for the project includes:

- Average tyre weight
- Number of tyres processed per day
- Daily production capacity in tons
- Number of pieces produced from each tyre
- Preprocessing stages
- Processing time assumptions
- Reactor batch capacity
- Reactor cycle time
- Product output assumptions
- Capital investment cost
- Operating cost assumptions
- Daily product profit assumptions
- Monitoring parameters for the mobile app

---

## Raw Data and Assumptions

### Production Assumptions

| Parameter | Value |
|---|---:|
| Average tyre weight | 10 kg |
| Tyres processed per day | 1000–1500 tyres |
| Daily production capacity | 10–15 tons/day |
| Pieces per tyre | 4 pieces |
| Total pieces per day | 4000–6000 pieces |
| Reactor capacity | 10 tons/batch |
| Reactor processing time | 18–23 hours/batch |

### Financial Assumptions

| Item | Value |
|---|---:|
| Estimated CAPEX | 700,000 JD |
| Expected net daily profit | 2,217 JD/day |
| Expected annual net profit | 798,120 JD/year |
| Expected payback period | 0.88 years |
| Expected ROI | 114% |

---

## Data Acquisition Method

The data was acquired through a combination of:

1. Project assumptions provided for the BioFuel system.
2. Literature-based ranges related to waste tyre pyrolysis and product recovery.
3. Estimated operational values suitable for a preliminary feasibility model.
4. Simulation logic requirements for building the process in Simio.
5. Financial scenario assumptions used to test conservative, expected, and optimistic cases.
6. Interface requirements for designing the digital monitoring app prototype.

---

## Data Reliability Notes

Some data values are based on assumptions and estimates because the project is a preliminary feasibility study. Therefore, the results should be treated as decision-support outputs rather than final industrial guarantees.

For real implementation, the following data should be validated:

- Actual machine processing times
- Real supplier quotations
- Real operating costs
- Market prices of pyrolysis oil, carbon black, and steel wires
- Product quality test results
- Environmental permit requirements
- Reactor downtime and maintenance records

---

## Data Storage in the Repository

The repository is organized to store data as follows:

| Folder | Purpose |
|---|---|
| `data/raw/` | Original assumptions, collected data, and raw input files |
| `data/processed/` | Cleaned or transformed data used for analysis |
| `notebooks/` | Python notebooks for financial and sensitivity analysis |
| `docs/` | Markdown documentation explaining data sources and methodology |

---

## Summary

The data research stage provided the foundation for the whole project. The collected values were used to define the simulation model, calculate system capacity, create financial scenarios, evaluate environmental benefits, and design the monitoring dashboard prototype.
