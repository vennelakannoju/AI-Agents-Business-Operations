# Employee Attrition Root-Cause Intelligence

**Domain:** HR

## Problem Statement

Employee turnover has increased significantly, creating recruitment costs and operational disruption. Develop an AI system that integrates employee performance, workload, compensation, absenteeism, overtime, engagement and training data to identify organizational factors associated with attrition and recommend evidence-based retention interventions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: reduce regretted attrition (high performers, critical roles). Guardrails: anonymize data, use job-related features only, no automated decisions on individuals.
2. Data Agent collects HRIS, pay, promotion, performance, overtime, absenteeism, engagement, training and exit data with restricted access.
3. Merge on an anonymized employee ID, mark leavers with the leaving date, and build features from before that date.
4. Train an attrition model with a time-based split; check results for bias across gender, age and other groups.
5. Use SHAP and group comparisons (e.g. attrition with vs without heavy overtime in the same department) to find the factors associated with leaving.
6. Insight Agent (LLM) analyzes exit interviews and survey comments and extracts themes: manager, growth, pay, workload.
7. Planner proposes interventions matched to each driver and compares their cost with the replacement cost of a leaver.
8. Human approval: HR head reviews. Actions are taken at team level; individual risk lists are visible only to HR partners.
9. Pilot the interventions in selected teams and keep similar teams as comparison.
10. Measure attrition and engagement after 3 to 6 months, then update the model and the interventions.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
