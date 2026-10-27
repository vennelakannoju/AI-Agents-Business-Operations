# Inventory Optimization

**Domain:** Operations

## Problem Statement

A retailer simultaneously experiences stockouts for high-demand products and excess inventory for slow-moving products. Develop an AI inventory intelligence system that analyzes historical demand, seasonality, sales, inventory and supplier lead times to recommend inventory decisions.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: raise in-stock rate and cut excess stock. Targets: e.g. 95% service level and fewer inventory days.
2. Data Agent pulls POS sales, stock by location, supplier lead times, prices and the promotion calendar.
3. Clean the data (treat stockout days as understated demand), then classify products by ABC (value) and XYZ (demand variability).
4. Forecast demand per product and store; backtest on recent weeks (WAPE) and compare against a simple baseline.
5. Set safety stock from forecast error and lead-time variability for the target service level; reorder point = demand during lead time + safety stock.
6. Calculate order quantity (EOQ) within supplier minimums and shelf-life limits.
7. Detect exceptions: stockout risk (stock cover below lead time) and overstock (cover above target); propose reorder, transfer or markdown.
8. Planner Agent (LLM) explains each recommendation in plain language and groups orders by supplier.
9. Buyer approves; routine reorders under a value limit are created automatically by the Action Agent as draft purchase orders.
10. Track stockout rate, inventory turns and excess stock; retune the model monthly.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
