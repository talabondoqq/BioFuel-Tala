# 04. Data Visualization and Dashboard Design

## Data Visualization and Insights

The project uses simulation screenshots, tables, charts, and dashboard visuals to communicate the main operational and business results of the BioFuel waste tyre pyrolysis system.

The visual analysis is important because it makes the relationship between process flow, capacity, bottlenecks, and business performance easier to understand.

---

## Main Visualization Areas

| Visualization Area | Purpose |
|---|---|
| Simio model layout | Shows the physical and logical production flow |
| Process flow diagram | Explains how tyres move through the system |
| Capacity comparison | Compares preprocessing capacity with reactor capacity |
| Utilization chart | Shows how busy each process is |
| Queue and waiting time chart | Identifies where material waits |
| Economic feasibility charts | Shows CAPEX, profit, payback, and ROI |
| Sensitivity analysis chart | Shows how risk affects profit |
| Product output distribution | Shows recovered products from pyrolysis |
| App prototype screens | Shows the digital monitoring concept |

---

## Simulation Visualization

The Simio model represents the system as a production process. Waste tyres enter the system, pass through preprocessing stages, and then move toward batching and reactor processing.

### Main Simio Components

| Component | Function |
|---|---|
| Source | Generates arriving waste tyres |
| Debeading | Removes steel wire from tyres |
| Cutting | Cuts tyres into smaller pieces |
| Shredding | Reduces tyre pieces into reactor-ready material |
| Buffer | Stores shredded material before batching |
| Parts Combiner | Combines pieces into full reactor batches |
| Oven / Reactor | Performs pyrolysis processing |
| Sink | Represents final system output |

---

## Process Flow Insight

The process flow shows that preprocessing stages are continuous, while the reactor works in batches. This creates a clear operational challenge: material can be prepared faster than the reactor can process it.

This is why the reactor is the main bottleneck in the system.

---

## Dashboard Design & Business Insights

A digital monitoring app prototype was created to show how BioFuel could monitor the plant in a simple and practical way.

The dashboard is designed to support managers and operators by showing important information such as machine status, reactor condition, material levels, alerts, reports, temperature, humidity, and production indicators.

---

## Dashboard Components

| Dashboard Component | Description | Business Insight |
|---|---|---|
| General Dashboard | Shows the overall system status | Helps users understand plant condition quickly |
| Reactor Dashboard | Tracks reactor status and batch condition | Focuses on the main bottleneck |
| Material Levels | Displays available and processed material | Supports batching and inventory control |
| Alerts and Reports | Shows warnings and operational notes | Helps respond faster to issues |
| Temperature and Humidity | Tracks operational environment indicators | Supports safer and more stable operation |
| Output Tracking | Shows product-related information | Connects production to business value |

---

## Business Questions Answered by the Dashboard

### Question 1: Is the system operating normally?

The general dashboard helps users check the status of the overall plant and identify whether any process requires attention.

### Question 2: What is happening in the reactor?

The reactor dashboard focuses on the most important part of the system. Since the reactor is the bottleneck, monitoring it helps reduce downtime and improve decision-making.

### Question 3: Is there enough material for batching?

Material level indicators help users understand whether the system has enough shredded material to form a full batch.

### Question 4: Are there any warnings?

Alerts and reports help identify operational problems early, such as delays, low material levels, or reactor-related issues.

---

## App Prototype Link

The digital monitoring prototype can be accessed here:

[BioFuel Monitoring App](https://iofuel.oneapp.dev/)

The application is a prototype for demonstration and decision-support purposes. It is not presented as a fully connected industrial control system.

---

## Key Visualization Insight

The most important insight from the visual analysis is that the reactor controls the system. Any improvement in reactor cycle time, capacity, or availability would improve production output, financial performance, and environmental benefit.
