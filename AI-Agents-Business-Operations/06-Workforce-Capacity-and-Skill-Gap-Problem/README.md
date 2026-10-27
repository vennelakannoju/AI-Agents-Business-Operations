# Workforce Capacity & Skill Gap Problem

**Domain:** HR

## Problem Statement

A company has sufficient employees on paper but continues to miss project deadlines because the required skills are not available at the right time. Develop an AI workforce intelligence system that maps employee skills against business requirements, identifies critical skill gaps, and recommends hiring, training and internal allocation strategies.

## 10-Step Solution Algorithm (AI Agent Workflow)

1. Set the goal: have the right skills available when projects need them. Metric: % of project-weeks fully staffed and on-time delivery.
2. Data Agent collects HR records, resumes, certifications, timesheets, current allocation, leave plans and the project pipeline.
3. Skill Extraction Agent (LLM) pulls skills and proficiency from resumes and project notes into a standard skill list; managers check a sample.
4. Build the demand table: for every project-week, the skill, level and hours required.
5. Build the supply table: available hours per skill-week = employees with the skill x (capacity - current allocation - leave).
6. Gap = demand - supply. Rank gaps by size, timing and revenue at risk.
7. Solve the matching: fill gaps first by internal reallocation, then by upskilling employees with adjacent skills, then by hiring or contractors.
8. Planner Agent (LLM) writes the plan with options, cost and timeline for each gap.
9. Human approval by HR and delivery heads; Action Agent creates allocation requests, training enrollments and job requisitions.
10. Track staffing coverage and deadlines met; refresh the skill map monthly.

---
*Course: AI Agents & Autonomous Business Operations, MBA 2025-2027, Woxsen University*
