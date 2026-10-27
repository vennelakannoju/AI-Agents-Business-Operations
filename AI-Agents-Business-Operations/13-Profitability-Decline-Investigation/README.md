# Profitability Decline Investigation

**Domain:** Business Analytics

## Problem Statement

Company profitability has declined for three consecutive quarters, but individual departments report satisfactory performance. Develop an AI business analyst that integrates Marketing, HR, Operations and Finance data to identify cross-functional relationships responsible for the decline.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: explain the three-quarter profit decline and find cross-functional causes.
2. Data Agent collects P&L (Finance), spend and discounts (Marketing), headcount, attrition and overtime (HR), costs, delays and returns (Operations).
3. Align data by quarter, product and region and reconcile totals with the Finance P&L.
4. Build a profit bridge: split the change into volume, price / discount, mix, cost of goods and operating cost effects.
5. Drill into the products, customers and regions that contribute most to the decline.
6. Test cross-department hypotheses with lagged correlation and regression (discounts -> margin; attrition -> delays -> refunds) and check that cause comes before effect.
7. Quantify each chain in money and rank them by profit impact.
8. Analyst Agent (LLM) writes the narrative with evidence and uncertainty, and proposes joint actions with owners and shared KPIs.
9. CFO and COO approve; Action Agent builds the cross-department dashboard and alerts; pilot the actions.
10. Review every quarter and check whether profit recovers as estimated.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
