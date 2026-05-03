# IAM Learning Assistant (AI Agent)

This project demonstrates the design and development of a declarative AI agent using Microsoft Copilot Studio.

## Overview
The IAM Learning Assistant helps users understand Identity and Access Management (IAM) concepts such as:
- Microsoft Entra ID
- Zero Trust
- Multi-Factor Authentication (MFA)
- Privileged Identity Management (PIM)

## Problem
IAM concepts are often complex and difficult for beginners due to technical documentation.

## Solution
This AI agent simplifies IAM topics by:
- Providing clear and short explanations
- Including real-world examples
- Using trusted sources (Microsoft Learn, NIST, OWASP)

## Features
- Beginner-friendly responses
- Structured explanations
- Guided prompts
- Handles irrelevant queries properly

## Testing
The agent was tested with:
- Relevant IAM-related questions
- Irrelevant questions to validate behavior

## Limitation
Publishing was not possible due to licensing restrictions, but the agent was fully built and tested.

## Author
Asad Majeed

## Architecture Diagram

```mermaid
flowchart LR
    User -->|Ask Question| Copilot[Copilot Studio Agent]
    Copilot --> Instructions[Agent Instructions]
    Copilot --> Knowledge[Knowledge Sources]
    Knowledge --> MS[Microsoft Learn]
    Knowledge --> NIST[NIST]
    Knowledge --> OWASP[OWASP]
    Copilot --> Response[Generated Response]
    Response --> User
