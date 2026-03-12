<div align="center">

<!-- Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=PhishMind&fontSize=72&fontColor=ffffff&fontAlignY=38&desc=AI-Powered%20Phishing%20Investigation%20Assistant&descSize=20&descAlignY=60&descColor=a78bfa" width="100%" alt="PhishMind Banner"/>

<br/>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

<br/>

![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square)
![Hackathon](https://img.shields.io/badge/Hack%20%26%20Break-GenAI%20%26%20Cybersecurity-blueviolet?style=flat-square)

<br/>

> 🛡️ **PhishMind** is a virtual cybersecurity analyst that investigates suspicious emails, URLs, and messages — and explains *why* they're dangerous.

</div>

---

## 📌 Table of Contents

- [Problem](#-problem)
- [Our Solution](#-our-solution)
- [Key Features](#-key-features)
- [System Workflow](#-system-workflow)
- [System Architecture](#-system-architecture)
- [Technology Stack](#-technology-stack)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)


---

## 🚨 Problem

Phishing attacks remain one of the most common and effective forms of cybercrime. Attackers impersonate trusted organizations — banks, social media platforms, delivery services — to trick users into revealing sensitive information.

Most cybersecurity tools only provide a **simple warning** with no explanation. This lack of transparency:

- ❌ Prevents users from understanding *how* phishing works
- ❌ Makes it difficult to build lasting digital awareness
- ❌ Leaves non-technical users confused and vulnerable

---

## 💡 Our Solution

PhishMind acts as a **virtual cybersecurity analyst** — investigating suspicious digital content step by step, then generating a human-readable report that explains every finding.

**Users can submit:**

| Input Type | Example |
|---|---|
| 📧 Suspicious email | Full email body with headers |
| 🔗 URL / link | `http://paypa1-secure-login.com/verify` |
| 💬 Text message | "Your package is on hold. Click here..." |
| 🌐 Website link | Any live URL to be analyzed |

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🤖 Automated Investigation | Full phishing analysis pipeline, no manual steps |
| 🧠 Explainable AI Reports | Understand *why* content is flagged, not just *that* it is |
| 🔍 Domain Reputation Analysis | Real-time domain age, registration, and reputation checks |
| 📊 Threat Scoring System | Risk scores with confidence levels per indicator |
| 🖥️ Non-Technical UI | Clean interface designed for everyday users |
| 🔗 Multi-Stage Pipeline | Layered analysis across URL, domain, page content, and AI |

---

## 🔄 System Workflow

```
┌─────────────────────────────────────────────────────────────┐
│                        USER INPUT                           │
│              Email / URL / SMS / Website                    │
└──────────────────────────┬──────────────────────────────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │    URL Extraction      │
              │  Extract all links &   │
              │  embedded domains      │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │  Domain Intelligence   │
              │  WHOIS · Age · Registr │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │  Threat Intelligence   │
              │  Reputation APIs &     │
              │  Blocklist Lookup      │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │  Webpage Analysis      │
              │  HTML parsing, forms,  │
              │  redirects & scripts   │
              └────────────┬───────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │   AI Reasoning Engine  │
              │  LLM synthesizes all   │
              │  signals into findings │
              └────────────┬───────────┘
                           │
                           ▼
┌─────────────────────────────────────────────────────────────┐
│                  EXPLAINABLE THREAT REPORT                  │
│         Risk Score · Indicators · Plain-English Summary     │
└─────────────────────────────────────────────────────────────┘
```

---

## 🏗️ System Architecture

```
┌──────────────────────────────────────┐
│         User Interface               │
│         React + Tailwind CSS         │
│         (Deployed on Vercel)         │
└─────────────────┬────────────────────┘
                  │  HTTP / REST
                  ▼
┌──────────────────────────────────────┐
│         Backend API                  │
│         Python + FastAPI             │
│         (Deployed on Render/Railway) │
└─────────────────┬────────────────────┘
                  │
        ┌─────────┴──────────┐
        │  Threat Analysis   │
        │     Modules        │
        ├────────────────────┤
        │  ├ URL Extractor    │
        │  ├ Domain Intel     │
        │  ├ Reputation Check │
        │  └ Webpage Analyzer │
        └─────────┬──────────┘
                  │
                  ▼
┌──────────────────────────────────────┐
│         AI Reasoning Engine          │
│     Groq / OpenAI / HuggingFace      │
└─────────────────┬────────────────────┘
                  │
                  ▼
┌──────────────────────────────────────┐
│         Security Report              │
│   Risk Score + Threat Indicators     │
│   + Plain-English Explanation        │
└──────────────────────────────────────┘
```

---

## 🛠️ Technology Stack

### 🖥️ Frontend
| Technology | Purpose |
|---|---|
| React | UI framework |
| Tailwind CSS | Styling & design system |
| Vercel | Deployment & hosting |

### ⚙️ Backend
| Technology | Purpose |
|---|---|
| Python | Core language |
| FastAPI | REST API framework |
| Render / Railway | Backend deployment |

### 🤖 AI Layer
| Technology | Purpose |
|---|---|
| Groq / OpenAI / HuggingFace | LLM-powered reasoning engine |

### 🔐 Security Analysis
| Library / Tool | Purpose |
|---|---|
| WHOIS lookup | Domain registration & age analysis |
| BeautifulSoup | HTML parsing & page structure |
| Domain analysis libraries | Typosquatting & DNS checks |
| Threat Intelligence APIs | Blocklist & reputation lookup |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- Node.js 18+
- API key for your chosen LLM provider

### Backend Setup

```bash
# Clone the repository
git clone https://github.com/your-username/phishmind.git
cd phishmind/backend

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
cp .env.example .env
# Add your API keys to .env

# Start the server
uvicorn main:app --reload
```

### Frontend Setup

```bash
cd phishmind/frontend

# Install dependencies
npm install

# Start the development server
npm run dev
```

---

## 📁 Project Structure

```
phishmind/
├── backend/
│   ├── main.py                   # FastAPI entry point
│   ├── routers/
│   │   └── analyze.py            # Analysis endpoints
│   ├── modules/
│   │   ├── url_extractor.py      # URL & link extraction
│   │   ├── domain_intel.py       # WHOIS & domain checks
│   │   ├── reputation.py         # Threat intelligence lookup
│   │   └── webpage_analyzer.py   # HTML structure analysis
│   ├── ai/
│   │   └── reasoning_engine.py   # LLM prompt & response
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/           # Reusable React components
│   │   ├── pages/                # App pages & routes
│   │   └── App.jsx
│   ├── tailwind.config.js
│   └── package.json
│
└── README.md
```

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=100&section=footer" width="100%" alt="footer"/>

<br/>

Made with 🛡️ by the **PhishMind Team**

</div>
