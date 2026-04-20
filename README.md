
# AI Risk Workflow Automation

AI-powered workflow system for automated classification, prioritization, and routing of insurance-related requests using LLMs, RAG, and workflow automation.

## Overview

This project demonstrates how AI can be applied to automate decision-making in insurance and risk management operations.

The system processes incoming unstructured messages such as client emails or support requests, converts them into structured data, and triggers appropriate business actions like routing, escalation, and notifications.

The goal is to reduce manual effort, improve response time, and ensure consistent handling of requests.

## Problem

Insurance and risk management teams handle a high volume of incoming requests, including:

- Claims (e.g., accidents, damages)  
- Risk alerts (e.g., cyber incidents, liability risks)  
- General inquiries  

These requests are typically:

- Unstructured in format  
- Time-sensitive  
- Processed manually  

This results in:

- Delays in response  
- Inconsistent prioritization  
- Increased operational workload  
- Risk of human error  

## Solution

This project implements an AI-driven workflow system that automates the end-to-end handling of incoming requests.

The system performs the following steps:

1. Receives incoming messages via webhook  
2. Uses an LLM-based triage agent to:
   - Classify requests (claim, risk, general)  
   - Assign priority levels (high, medium, low)  
   - Identify risk type (cyber, liability, property)  
3. Enhances decision-making using Retrieval-Augmented Generation (RAG) for contextual understanding  
4. Routes requests to the appropriate teams using APIs and webhooks  
5. Triggers real-time notifications for high-priority cases  
6. Stores and logs all processed data for tracking and evaluation  

## Architecture

Incoming Request (Webhook)
↓
Preprocessing
↓
RAG (Context Retrieval)
↓
LLM Triage Agent
↓
Decision Engine
↓
API Actions (Routing / Alerts)
↓
Logging and Storage
