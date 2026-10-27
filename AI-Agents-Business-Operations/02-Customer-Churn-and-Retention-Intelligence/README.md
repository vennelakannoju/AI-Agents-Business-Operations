# Customer Churn & Retention Intelligence

**Domain:** Marketing

## Problem Statement

A subscription business is experiencing increasing customer churn despite continued marketing expenditure. Develop an AI system that identifies behavioral patterns associated with churn, segments at-risk customers, determines potential causes, and generates personalized retention strategies.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: reduce voluntary churn at an acceptable retention cost. Define churn (no renewal within 30 days of expiry) and cap offers at customer margin.
2. Data Agent collects subscription, usage logs, billing, support tickets and survey (NPS) data for each customer.
3. Build features using only information available before the churn date (avoids leakage): usage trend, days since last login, failed payments, tickets, plan, tenure.
4. Train a churn model with a time-based split (older months to train, latest months to test); use class weights for imbalance; judge by AUC and recall in the top 10% risk.
5. Explain with SHAP and cluster the at-risk customers (K-Means) into segments with different churn drivers.
6. Planner Agent (LLM) reads each segment's tickets and reviews to find reasons for leaving, and retrieves the company's retention playbook (RAG).
7. Planner drafts a personalized action per segment: offer, message, channel and timing, within the cost limit.
8. Human approval: retention manager reviews templates. Low-cost actions go out automatically; large discounts need approval.
9. Action Agent sends the messages through CRM / email; a random 10% of at-risk customers receive nothing, as a control group.
10. Measure uplift = churn of control minus churn of treated customers, net of cost. Feed results back and retrain monthly.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
