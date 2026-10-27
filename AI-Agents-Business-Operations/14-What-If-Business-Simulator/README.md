# What-If Business Simulator

**Domain:** Business Analytics

## Problem Statement

Management wants to increase sales by 20% but does not know whether existing employees, inventory, production capacity and logistics can support the additional demand. Build an AI scenario-analysis system that simulates business consequences of different strategic decisions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: test whether a 20% sales increase is feasible. Define the scenario: timeline, product mix and price.
2. Data Agent collects sales, staffing, inventory and lead times, production capacity, logistics capacity and costs.
3. Build a driver-based model: units sold -> labor hours, materials, machine hours, deliveries; calibrate it against past data.
4. Forecast baseline demand and apply the uplift (run 10%, 20% and 30% scenarios).
5. Simulate month by month the utilization of each resource; use Monte Carlo for uncertainty in demand and lead time.
6. Identify the bottleneck: the first resource to pass full (or 85%) utilization, and when.
7. Cost the options to remove it (hire, overtime, extra shift, outsource, buffer stock, extra transport) and compute the effect on margin.
8. Scenario Agent (LLM) turns a manager's question (e.g. '+20% sales with 10% fewer staff') into model inputs, runs the simulation and explains results with numbers.
9. Management compares scenarios on profit, risk, cost and time, and approves one plan.
10. Monitor actual vs simulated results and recalibrate the model.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
