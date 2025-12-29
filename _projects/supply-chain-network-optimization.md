---
title: "Multi-Echelon Supply Chain Network Flow Optimization"
collection: projects
permalink: /projects/supply-chain-network-flow-optimization/
excerpt: "Graduate optimization project formulating a multi-echelon supply chain network flow model to minimize transportation cost under supply, demand, and capacity constraints."
github_url: "(https://github.com/JuanJ-MG/supply-chain-network-optimization)"
share: false
comments: false
---

## Resources

- **GitHub repository :**  
  👉 [Multi-Echelon Supply Chain Network Flow Optimization](https://github.com/JuanJ-MG/supply-chain-network-optimization)

---

## Overview

This project formulates and solves a **multi-echelon supply chain optimization problem** that determines how products should flow through a distribution network to minimize total transportation cost.

The system consists of **suppliers, distribution centers, and customers**, with products flowing from suppliers to distribution centers and then onward to customers. The model focuses on **quantity flow decisions**, ensuring that all customer demand is satisfied while respecting supply availability and capacity limits across the network.

The project was developed as a **final project for a graduate-level Supply Chain / Optimization course**.

---

## Problem Description

The planning problem integrates **flow allocation and capacity management** decisions:

- Suppliers have limited production capacity
- Distribution centers have throughput capacity constraints
- Customers have fixed demand requirements
- Transportation between nodes incurs cost

The objective is to determine how much product should be shipped along each link in the network so that demand is met at minimum total cost.

---

## Network-Based Formulation

The model is formulated as a **static network flow optimization problem**:

- Nodes represent supply, transshipment, and demand points
- Arcs represent transportation links with associated costs
- Decision variables represent shipment quantities on each arc

All decisions are made for a **single planning period**, with no explicit modeling of time, inventory carryover, or sequencing.

---

## Objective Function

The objective is to minimize **total system transportation cost**, accounting for:

- Shipments from suppliers to distribution centers
- Shipments from distribution centers to customers

This structure allows the model to identify cost-efficient flow patterns across the entire supply chain.

---

## Constraints

Key constraints in the model include:

- Supplier production capacity limits
- Distribution center throughput capacity limits
- Flow conservation at distribution centers
- Full satisfaction of customer demand

Together, these constraints ensure a feasible and economically efficient supply chain configuration.

---

## Solution Approach

The resulting model is a **linear programming (LP) formulation** with a network flow structure. The formulation is solved using standard optimization solvers, yielding globally optimal shipment decisions.

Because the model is static and single-period, it is computationally efficient and well-suited for tactical supply chain planning and cost analysis.

---

## Implementation

- **Model type:** Static multi-echelon network flow model
- **Decision structure:** Shipment quantity allocation
- **Tools:** Python, Jupyter Notebook, optimization solver
- **Application context:** Supply chain distribution planning

---

## Applicability

Although motivated by a generic supply chain setting, the formulation is directly applicable to a wide range of **industrial and aerospace logistics problems**, including:

- Spare parts distribution networks
- Manufacturing-to-assembly supply chains
- MRO logistics planning
- Defense and aerospace distribution systems
- Strategic and tactical transportation planning

The structure closely parallels many real-world logistics systems where **cost-efficient flow allocation** is critical.


---

*This project demonstrates the use of network flow optimization models to support cost-effective supply chain planning in complex, capacity-constrained distribution systems.*
