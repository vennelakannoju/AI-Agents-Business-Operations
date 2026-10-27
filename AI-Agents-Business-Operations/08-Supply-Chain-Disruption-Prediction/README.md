# Supply Chain Disruption Prediction

**Domain:** Operations

## Problem Statement

A manufacturing company frequently experiences production delays because disruptions in suppliers, inventory and transportation are identified too late. Develop an AI operations system that analyzes supplier, inventory, production and delivery data to identify emerging risks and recommend mitigation actions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: detect supply disruptions 2 to 4 weeks early. Define disruption: delivery over 2 days late, stock below safety level or a production stoppage.
2. Data Agent connects ERP (orders, inventory), supplier delivery history, production plan, shipment tracking and news / weather feeds.
3. Build a supplier-material-week table with the label 'disruption in the next 14 to 28 days'.
4. Create features: delay trend, days of stock cover, order backlog, transit-time variation, supplier concentration, external alerts.
5. Train a classifier with a time-based split and class weights (disruptions are rare); pick the alert threshold that balances missed events and false alarms.
6. Monitoring Agent (LLM) scans news and supplier emails for risk events and links them to affected suppliers and materials.
7. Risk score = probability x production impact (units or revenue at stake); rank the top risks.
8. Planner proposes mitigations with cost and time (alternate supplier, buffer stock, expedite, reroute) and picks the cheapest that protects production.
9. Human approval by the planner; Action Agent drafts the purchase order or expedite request and alerts the team (automatic only for low-cost actions).
10. Log outcomes, measure precision and recall, and retrain monthly.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
