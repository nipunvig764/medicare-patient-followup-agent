# MediCare Patient Follow-Up Agent

An Agentic AI prototype that helps healthcare care-coordination teams identify patients requiring follow-up, prioritize them, and generate recommended follow-up actions.

## Problem Statement

Healthcare teams managing large numbers of chronic-disease patients may struggle to continuously review patient records. Missed appointments or concerning patient information may therefore not receive timely attention.

This project builds an AI-powered patient follow-up agent that can:

- Analyze patient records
- Identify missed appointments
- Prioritize patients for follow-up
- Generate risk summaries and recommended actions
- Support individual patient analysis
- Expose the workflow through REST APIs

## Architecture

```text
Patient Data (CSV)
       |
       v
Agent Tools
       |
       v
Groq LLM Agent
       |
       | Selects required tool
       v
Tool Execution
       |
       v
Patient Context
       |
       v
LLM Reasoning
       |
       v
Priority + Risk Summary
+ Recommended Follow-up Actions
       |
       v
FastAPI
