# ☢️ Core Reactor Management System (Gemini AI)

A high-tech terminal interface powered by **Google Gemini 2.0 Flash** and **Gradio**. This application monitors simulated reactor status, handles local override commands, and features an automated emergency alert system for high-heat detection.

## ✨ Features
* **Gemini AI Integration:** Uses state-of-the-art LLM for intelligent system responses.
* **Emergency Detection:** Real-time logic scans outputs for "High Heat" or "Coolant" issues.
* **Gradio UI:** A "Glass" themed, responsive web interface.
* **Safety Metadata Filtering:** Clean chat output (no "Safety Cleared" technical clutter).
* **Local Override Mode:** Specialized system prompts for reactor simulation.

---

## 🚀 Quick Start

### 1. Prerequisites
* Python 3.9+
* A Gemini API Key (Get it at [Google AI Studio](https://aistudio.google.com/))

### 2. Installation
Clone the repository and install the dependencies:
```bash
pip install google-genai gradio python-dotenv

```

### 3. Configuration

Create a `.env` file in the root directory and add your API key:

```env
GEMINI_API_KEY=your_actual_key_here

```

### 4. Run the App

```bash
python app.py

```

The interface will be available at `http://127.0.0.1:7860`

---

## 🛠️ Project Structure

* **app.py**: The main application logic and Gradio UI.
* **.env**: (Hidden) Stores your private API credentials.
* **requirements.txt**: List of necessary Python packages.

## ⚠️ System Alerts

The system is programmed to trigger a **UI Warning Banner** if any of the following keywords are detected in the reactor output:

* `High Heat`
* `Emergency`
* `Coolant Flow`
* `Pressure Vent`

---
---

---

---

## 🚀 Live Demo

You can test the **Core Reactor Management System** live on Hugging Face Spaces. The interface allows you to simulate reactor conditions and observe the Agentic AI's safety responses in real-time.

[![Open in Spaces](https://huggingface.co/datasets/huggingface/badges/resolve/main/open-in-hf-spaces-lg-dark.svg)([https://huggingface.co/spaces/YOUR_USERNAME/YOUR_SPACE_NAME](https://priyanshu-kumar-001-ai-reliability-agent.hf.space/?__theme=system&deep_link=3a3Au1WFODQ))]
](https://priyanshu-kumar-001-ai-reliability-agent.hf.space/?__theme=system&deep_link=3a3Au1WFODQ)
> **Pro Tip:** If the Space is "Sleeping," simply click the link and wait a few moments for the container to restart.

---
---
