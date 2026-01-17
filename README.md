
# AI-Reliability: Agentic Control for Tennessee Eastman Reactor

This project demonstrates a **Hybrid Intelligent System** for industrial fault detection and recovery. It combines traditional Machine Learning (Random Forest) with Large Language Models (Gemini 1.5 Flash) to monitor and manage a chemical reactor based on the **Tennessee Eastman Process (TEP)** benchmark.

## 🚀 Key Features

* **Real-time Fault Detection:** A Random Forest classifier trained on TEP sensor distributions (Temperature, Pressure, and Flow) to identify process deviations.
* **Agentic Reasoning:** An LLM-based controller that interprets sensor data and generates natural language engineering instructions.
* **Physics-Informed Safety Interlock:** A deterministic logic layer that monitors AI commands. If the AI suggests an action that violates industrial safety physics (e.g., closing a valve during a high-pressure event), the system triggers a **Self-Correction** loop.
* **Industrial Dashboard:** A dark-mode DCS (Distributed Control System) interface built with Gradio, featuring multivariate radar charts for process health visualization.

## 🏗️ System Architecture

The system operates in three distinct layers to ensure maximum reliability:

1. **Perception Layer:** Scaled sensor inputs are processed by a scikit-learn model to detect anomalies.
2. **Cognition Layer:** Google Gemini 1.5 Flash analyzes the state vs. Standard Operating Procedures (SOPs).
3. **Safety Layer:** A hard-coded "Interlock" validates AI instructions against safety thresholds before execution.

## 🛠️ Tech Stack

* **Language:** Python
* **AI/LLM:** Google Gemini 1.5 Flash (via Google Generative AI API)
* **Machine Learning:** Scikit-Learn (Random Forest, StandardScaler)
* **Interface:** Gradio
* **Visualization:** Plotly (Radar Charts), Matplotlib (Sensitivity Analysis)
* **Data:** Tennessee Eastman Process (TEP) calibrated distributions

## 📋 Installation & Usage

### 1. Clone the repository

```bash
git clone https://github.com/your-username/tep-ai-reliability.git
cd tep-ai-reliability

```

### 2. Install dependencies

```bash
pip install gradio google-generativeai plotly scikit-learn pandas numpy

```

### 3. Configure API Key

Get an API key from [Google AI Studio](https://aistudio.google.com/) and add it to your environment variables or directly in the configuration cell:

```python
genai.configure(api_key="YOUR_API_KEY")

```

### 4. Run the Project

Open the notebook in Google Colab or run the script:

```bash
python app.py

```

## 📊 Industrial Context

The **Tennessee Eastman Process** is a world-renowned benchmark in the chemical engineering community used to evaluate process control and monitoring systems. This project applies modern "Agentic AI" to this classic problem, showcasing how LLMs can assist human operators in high-stakes environments without compromising safety.

---

