---
title: "Two-Stage Stochastic Manufacturing Planning with Benders Decomposition"
collection: projects
permalink: /projects/two-stage-stochastic-manufacturing-planning/
excerpt: "Graduate optimization project modeling long-term AM/TM capacity investment and short-term production planning under uncertain demand using Benders decomposition."
github_url: "https://github.com/JuanJ-MG/two-stage-stochastic-manufacturing-benders-decomposition"
share: false
comments: false
---

## Overview

This project studies a **two-year manufacturing planning problem** motivated by **aircraft spare-parts supply chains**.  
The system faces long-term capacity investment decisions under uncertainty, followed by short-term operational planning after demand is realized.

The project was developed as the **final project for a graduate-level Advanced Systems Optimization course**.

---

## Problem Description

The planning horizon is divided into two stages:

### Year 1 – Strategic Investment Decisions
- Decide how many machines to purchase
- Technologies include:
  - **Additive Manufacturing (AM)**
  - **Traditional Manufacturing (TM)**
- Investment decisions are:
  - Capital-intensive
  - Long-term
  - Integer-valued and irreversible

### Year 2 – Operational Decisions under Uncertainty
Once demand is realized, the system decides:
- Production quantities
- Labor and overtime usage
- Short-term capacity additions
- Penalties for unmet demand

---

## Demand Uncertainty

- Year-2 demand is uncertain
- Represented using **multiple demand scenarios**
- Each scenario has an associated probability
- Objective is to **minimize expected total cost** across scenarios

---

## Objective Function

The model minimizes **expected total system cost**, including:

- Machine investment costs (Year 1)
- Operating and labor costs (Year 2)
- Overtime and short-term capacity costs
- Penalties for unmet demand

All decisions are subject to:
- Budget constraints
- Labor availability constraints
- Capacity and production limits

---

## Solution Approach

To solve the problem efficiently, the model is implemented using **Benders decomposition**:

- The **master problem** determines Year-1 investment decisions
- **Subproblems** solve Year-2 operational planning for each demand scenario
- Cuts are iteratively added to coordinate strategic and operational decisions

This decomposition allows:
- Handling multiple demand scenarios
- Keeping investment decisions integer-valued
- Solving large-scale stochastic MILPs efficiently

---

## Implementation

- **Model type:** Two-stage stochastic MILP
- **Solution method:** Benders decomposition
- **Tools:** Python, Gurobi
- **Formulation:** Scenario-based stochastic optimization

---

## Applicability

Although motivated by **aircraft manufacturing and spare-parts supply chains**, the formulation and solution approach are broadly applicable to:

- Logistics and distribution planning
- Infrastructure investment under uncertainty
- Capacity planning with long-term commitments
- Resource-constrained systems with stochastic demand

---

## Resources

- **Code and implementation:**  
  👉 [GitHub repository]({{ page.github_url }})

---

*This project demonstrates the application of stochastic optimization and decomposition techniques to complex, multi-stage decision-making problems under uncertainty.*
