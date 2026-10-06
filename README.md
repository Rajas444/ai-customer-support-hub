# AI-Powered Customer Support Automation & Analytics Hub

An industry-focused full-stack automation platform built for modern enterprise customer management ecosystems. The application seamlessly integrates Large Language Models (LLMs) with robust transactional tracking and telemetric data reporting to automate operational customer workflows.

## 🚀 Core Architectural Features
* **Automated Support Workflows:** Processes multi-turn customer tickets 24/7, cross-referencing incoming complaints with a structured, local product knowledge base.
* **LLM Engineering & Structured Schemas:** Executes complex parameter prompts using strict system instructions to guarantee predictable structured JSON data extraction.
* **Real-Time Sentiment Classification:** Monitors real-time semantic patterns in customer queries to classify sentiment and dynamically trigger emergency human agent webhooks on critical distress flags.
* **Resilient Offline Architecture:** Engineered with an automated local regex/keyword-matching fallback mechanism to seamlessly process workflows during API timeout events or network spikes.
* **Interactive Telemetry Dashboard:** Implements instantaneous management tracking interfaces evaluating high-level Key Performance Indicators (KPIs) like absolute customer health indexes and escalation percentages.

## 🛠️ System Tech Stack
* **UI/UX Design Framework:** Streamlit (Python UI Engine)
* **AI Cognitive Processing Suite:** Google Gemini SDK (`gemini-2.5-flash`)
* **Persistence & Transaction Engine:** SQLite3 Relational Database Layer
* **Application Script Engine:** Python 3.x

## 💻 Local Installation & Setup Guide

1. **Clone the Repository Workspace:**
   ```bash
   git clone https://github.com
   cd ai-customer-support-hub
   ```

2. **Install Application Dependencies:**
   ```bash
   pip install streamlit google-genai
   ```

3. **Acquire Access Credentials:**
   * Visit [Google AI Studio](https://google.com) and authorize access using a standard Google profile.
   * Generate a development API token and copy it securely into your local configurations.

4. **Boot Up the Application Server:**
   ```bash
   python -m streamlit run app.py
   ```

## 📊 Relational Database Visual Blueprint
The system uses an autonomous embedded SQLite transactional database mapping two primary entity-relationship architectures:
* `tickets`: Main relational log managing entries for `customer_name`, raw `query` objects, processed AI `response` arrays, `sentiment` classes, and resolution `status` markers.
* `knowledge_base`: Anchors the structural validation domain containing explicit enterprise operating facts (`topic`, `details`) referenced directly by the LLM system prompts.
