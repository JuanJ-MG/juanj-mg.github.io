---
title: "Time-Indexed MILP Assignment and Scheduling with Travel Costs"
collection: projects
permalink: /projects/time-indexed-assignment-scheduling-travel/
excerpt: "Graduate optimization project formulating a time-indexed MILP for assignment and scheduling with travel-dependent sequencing costs."
github_url: "(https://github.com/JuanJ-MG/OR/Systems Optimization/Final Project)"
share: false
comments: false
---

## Resources

- **GitHub repository :**  
  👉 [Time-Indexed MILP Assignment and Scheduling with Travel Costs](https://github.com/JuanJ-MG/OR/Systems Optimization/Final Project)

---

## Overview

This project formulates and solves a **time-indexed mixed-integer linear programming (MILP)** model for an **assignment and scheduling problem with travel costs**, motivated by the scheduling of **professors traveling between campuses to teach courses over a discrete planning horizon**.

The system must assign professors to teaching tasks at specific times while respecting availability, task durations, and sequencing constraints. Because professors may need to travel between locations, scheduling decisions are tightly coupled with **travel feasibility and travel-dependent costs**, resulting in a spatiotemporal optimization problem.

The project was developed as a **final project for a graduate-level Systems Optimization course**.

---

## Problem Description

The planning problem integrates **assignment, sequencing, and timing** decisions:

- Professors must be assigned to teaching tasks
- Each task has a fixed time window and duration
- Professors cannot be assigned to overlapping tasks
- Travel between consecutive tasks incurs costs and time penalties

The formulation explicitly captures the interaction between **where** a task is performed and **when** it is scheduled.

---

## Time-Indexed Formulation

The model uses **time-indexed decision variables** to represent whether a professor is assigned to a specific task at a given time period. This formulation ensures:

- Temporal feasibility of assignments
- Prevention of overlapping tasks
- Correct sequencing of tasks over time

Travel costs are introduced between consecutive assignments, linking spatial transitions with temporal decisions and penalizing inefficient sequences.

---

## Objective Function

The objective is to minimize **total system cost**, which includes:

- Assignment costs
- Travel costs between consecutive tasks
- Penalties for infeasible or poorly sequenced schedules

This structure allows the optimization to balance efficient use of resources with coherent travel and timing decisions.

---

## Constraints

Key constraints in the model include:

- Assignment feasibility and exclusivity
- Time-window and duration constraints
- Sequencing constraints between tasks
- Travel feasibility between locations
- Resource availability constraints

Together, these constraints enforce a globally feasible and efficient schedule.

---

## Solution Approach

The resulting model is a **large-scale time-indexed MILP**, solved using commercial optimization software. The time-indexed structure enables precise modeling of temporal interactions but requires careful formulation to manage model size and computational complexity.

---

## Implementation

- **Model type:** Time-indexed MILP
- **Decision structure:** Assignment, sequencing, and timing
- **Tools:** Python, Gurobi
- **Application context:** Faculty scheduling with travel considerations

---

## Applicability

Although motivated by an academic scheduling application, the formulation is directly applicable to a broad class of **aerospace and space logistics problems**, including:

- Space mission campaign planning
- Spacecraft task scheduling
- Crew and asset assignment over time
- Multi-node logistics in multi-planetary systems
- Operations planning with transition costs and timing constraints

The model structure closely parallels problems in **space mission operations and autonomy**, where agents or assets must be scheduled over time while accounting for **movement, sequencing, and limited resources**.

---

---

*This project demonstrates the use of time-indexed MILP formulations for integrated assignment, scheduling, and travel-cost optimization in complex, resource-constrained systems.*
