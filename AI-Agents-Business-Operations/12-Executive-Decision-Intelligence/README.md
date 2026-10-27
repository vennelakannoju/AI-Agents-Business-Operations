# Executive Decision Intelligence

**Domain:** Business Analytics

## Problem Statement

Senior management receives hundreds of KPIs from different departments but cannot identify which indicators actually explain changes in business performance. Develop an LLM-powered decision-intelligence system that connects operational KPIs with financial outcomes and generates evidence-based executive insights.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: identify the few KPIs that really explain changes in revenue and profit. Select the financial outcomes to explain.
2. Data Agent collects KPIs from Marketing, HR, Operations and Finance into one KPI table with a data dictionary.
3. Standardize definitions and periods; remove duplicate or highly correlated KPIs and shortlist about 20 to 30, because there are few time periods.
4. Run lagged correlations and a regularized regression (Lasso) to find candidate drivers; check stability with cross-validation.
5. Validate candidates with lag tests (Granger) and business logic; call them predictive drivers unless confirmed by an experiment.
6. Build a driver tree: operational KPI -> intermediate KPI -> financial outcome, with estimated effect sizes.
7. Insight Agent (LLM) with access to the KPI table and driver model answers questions (e.g. 'why did margin fall?') using retrieved numbers only.
8. Planner generates a weekly executive brief: top changes, drivers, recommended action and confidence level.
9. Executives review and give feedback; Action Agent assigns follow-up tasks to KPI owners.
10. Track decisions and results, and refresh the driver model every quarter.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
