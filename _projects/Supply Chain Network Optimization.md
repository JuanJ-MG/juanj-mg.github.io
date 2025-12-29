---
title: "Supply Chain Network Optimization"
categories: [Optimization, Supply Chain]
tags: [Linear Programming, Logistics]
---

## Overview

This project solves a **supply chain distribution problem** by determining how products should flow from suppliers to distribution centers and then to customers. The objective is to **minimize total transportation cost** while ensuring that all customer demand is satisfied and operational limits are respected.

The model represents a **static, single-period supply chain** and focuses on quantity decisions rather than routing or scheduling.

---

## What the Model Does

The optimization model decides:
- How much product to ship from each supplier to each distribution center
- How much product to ship from each distribution center to each customer

All flows are optimized simultaneously to achieve the lowest total cost.

---

## System Structure

The supply chain consists of:
- Suppliers with limited production capacity
- Distribution centers with throughput limits
- Customers with fixed demand

Products move through the network in two stages: supplier → distribution center → customer.

---

## Constraints

The model enforces:
- Supplier capacity limits
- Distribution center capacity limits
- Flow balance at distribution centers
- Full satisfaction of customer demand

---

## Model Characteristics

- **Problem type:** Supply chain network flow
- **Time representation:** None (single-period, static)
- **Decision focus:** Shipment quantities
- **Solution method:** Linear optimization

This is **not** a routing, scheduling, or time-expanded model.

---

## Results

The optimized solution provides:
- Optimal shipment quantities on each supply chain link
- Minimum achievable transportation cost
- Clear insight into how demand is served through the network

---

## Why This Matters

Models like this are widely used in:
- Logistics and distribution planning
- Manufacturing supply chains
- Cost-reduction and capacity planning studies

This project demonstrates how optimization can support **data-driven supply chain decisions** in complex distribution networks.

---

## Tools Used

- Python
- Jupyter Notebook
- Gurobi
