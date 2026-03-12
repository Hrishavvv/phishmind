# PhishMind
### AI-Powered Phishing Investigation Assistant

PhishMind is an AI-powered cybersecurity assistant designed to investigate suspicious emails, URLs, and messages. Instead of simply labeling content as *safe* or *malicious*, the system performs a structured investigation and explains **why** the content may be dangerous.

The goal of PhishMind is to make cybersecurity investigation understandable for everyday users by combining automated security analysis with explainable AI reasoning.

This project is being developed for the **Hack & Break: Generative AI & Cybersecurity Innovation Challenge**.

---

# Problem

Phishing attacks remain one of the most common and effective forms of cybercrime. Attackers often impersonate trusted organizations such as banks, social media platforms, or delivery services to trick users into revealing personal information.

Although many cybersecurity tools can detect malicious content, most of them only provide a simple warning without explaining the reasoning behind the detection. This lack of transparency prevents users from learning how phishing attacks work and makes it harder to build digital awareness.

---

# Our Solution

PhishMind acts as a **virtual cybersecurity analyst** that investigates suspicious digital content step by step.

Users can submit:

- suspicious emails
- URLs
- text messages
- website links

The system then analyzes the content through multiple technical checks and generates a **clear security report** describing the risk level and detected indicators.

---

# System Workflow

The platform follows a structured investigation pipeline:
User Input
↓
URL Extraction
↓
Domain Intelligence Check
↓
Threat Intelligence Lookup
↓
Webpage Structure Analysis
↓
AI Reasoning Engine
↓
Explainable Threat Report


Each stage collects technical signals that help determine whether the content may be part of a phishing attempt.

---

# Key Features

• Automated phishing investigation  
• Explainable AI security reports  
• Domain reputation analysis  
• Threat scoring system  
• Simple user interface for non-technical users  
• Multi-stage cybersecurity analysis pipeline  

---

# Technology Stack

## Backend
- Python
- FastAPI

## Frontend
- React
- Tailwind CSS

## AI Layer
- Cloud-hosted LLM (Groq / OpenAI / HuggingFace)

## Security Analysis
- WHOIS lookup
- HTML parsing using BeautifulSoup
- Domain analysis libraries
- Threat intelligence APIs

## Deployment
- Backend: Render / Railway
- Frontend: Vercel

---

# System Architecture


User Interface (React)
↓
Backend API (FastAPI)
↓
Threat Analysis Modules
│
├ URL Extractor
├ Domain Intelligence Check
├ Reputation Lookup
└ Webpage Analyzer
↓
AI Reasoning Engine
↓
Security Report
