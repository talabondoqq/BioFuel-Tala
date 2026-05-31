# 05. Advanced Analytics and AI Modeling

## Overview

The advanced analytics part of this project focuses on financial scenario analysis and sensitivity testing. The goal is to evaluate whether the proposed BioFuel waste tyre pyrolysis system remains feasible under different economic conditions.

Instead of using a complex machine learning model, this project uses a decision-support financial model. This approach is suitable because the main question is not prediction from a large dataset, but feasibility under different assumptions.

---

## Purpose of the Advanced Analytics Model

The advanced analytics model was designed to answer the following questions:

1. What is the expected profitability of the project?
2. How long does it take to recover the initial investment?
3. How sensitive is the project to changes in costs and product profit?
4. What are the most important financial risk factors?
5. Is the project still feasible under conservative assumptions?

---

## Main Financial Inputs

| Input | Value |
|---|---:|
| Estimated CAPEX | 700,000 JD |
| Expected net daily profit | 2,217 JD/day |
| Expected annual net profit | 798,120 JD/year |
| Expected payback period | 0.88 years |
| Expected ROI | 114% |

---

## Scenario Analysis

The model evaluates three main scenarios:

| Scenario | Description |
|---|---|
| Conservative | Lower revenue or higher risk case |
| Expected | Most realistic assumed case |
| Optimistic | Higher revenue or better operating case |

### Scenario Results

| Scenario | Net Daily Profit | Monthly Net Profit | Annual Net Profit | Payback Period | ROI |
|---|---:|---:|---:|---:|---:|
| Conservative | 1,817 JD | 54,510 JD | 654,120 JD | 1.07 years | 93.45% |
| Expected | 2,217 JD | 66,510 JD | 798,120 JD | 0.88 years | 114.02% |
| Optimistic | 2,617 JD | 78,510 JD | 942,120 JD | 0.74 years | 134.59% |

---

## Sensitivity Analysis

Sensitivity analysis was used to test how changes in cost and profit affect the feasibility of the project.

The analysis considered:

- Higher operating costs
- Lower product profit
- Conservative selling prices
- Reactor downtime risk
- Product quality risk
- Market demand changes

---

## Most Important Risk Drivers

| Risk Variable | Effect on Feasibility |
|---|---|
| Pyrolysis oil price | Very high |
| Daily production rate | Very high |
| Reactor downtime | High |
| Product quality | High |
| Labor and energy cost | Medium |
| Market access | High |

---

## Main Advanced Analytics Insight

The most important insight is that the project is financially promising under the expected assumptions, but profitability depends heavily on reactor reliability and product selling prices.

The reactor affects the project in three ways:

1. It controls daily throughput.
2. It affects daily product output.
3. It directly affects revenue and payback period.

Because of this, reducing reactor downtime or increasing reactor capacity would improve the financial feasibility of the project.

---

## AI and Decision-Support Value

The digital monitoring app adds decision-support value by helping operators monitor important system indicators. In future development, AI features could be added to predict maintenance needs, detect abnormal reactor behavior, or estimate production delays.

Possible future AI features include:

- Reactor downtime prediction
- Maintenance alerts
- Product output forecasting
- Energy consumption monitoring
- Anomaly detection
- Automated reporting

---

## Conclusion

The advanced analytics results support the overall feasibility of the project. The expected scenario shows a short payback period and strong ROI. However, the project should be validated with real market prices, operating data, supplier quotations, and product quality testing before final investment.
