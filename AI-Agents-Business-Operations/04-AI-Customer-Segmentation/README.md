# AI Customer Segmentation

**Domain:** Marketing

## Problem Statement

A company treats its customers using broad demographic segments, resulting in inefficient campaigns. Develop an LLM-powered customer intelligence system that discovers meaningful behavioral segments from transaction and interaction data and recommends differentiated marketing strategies.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: replace demographic segments with behavioral segments that raise response rate and revenue per customer.
2. Data Agent pulls transactions, website / app activity, support chats, reviews and past campaign responses.
3. Build one row per customer: recency, frequency, spend, category mix, discount use, channel preference, returns.
4. Convert chats and reviews to text embeddings, reduce them (PCA / UMAP), then scale and combine with the numeric features.
5. Cluster with K-Means; choose k using silhouette score and business usefulness; check that clusters stay stable on a different sample.
6. Profile each cluster: size, revenue share, margin, churn rate and growth.
7. Segment Agent (LLM) names each segment, describes it and proposes a strategy: offer, channel, timing and message.
8. Human approval: marketing manager edits the strategies and brand / compliance checks them.
9. Action Agent loads segment audiences into the email / ad tool and runs an A/B pilot: segment-based vs current campaign.
10. Compare response and revenue uplift; re-cluster every quarter and track customers moving between segments.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
