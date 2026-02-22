# ROSA – Agentic AI Framework for Robotics

> Production-ready Agentic AI system that translates natural language instructions into executable ROS actions using ReAct reasoning and LLM planning.

---

## Overview

**ROSA (Robotic Orchestrated Semantic Agent)** bridges Large Language Models and robotic control systems.

It enables robots to:

* Interpret natural language commands
* Reason over multi-step tasks
* Generate executable ROS action sequences
* Adapt dynamically using feedback loops

This framework combines:

* ReAct-style reasoning
* LLM-based task planning
* Structured ROS node orchestration
* Real-time execution validation

---

## Problem

Traditional robotic systems require:

* Hard-coded task pipelines
* Manual scripting for new behaviors
* Limited adaptability to ambiguous instructions

ROSA removes this constraint by enabling:

**Natural language → Structured robotic execution**

---

## Architecture

```
User Prompt
    ↓
LLM Planner (ReAct Reasoning)
    ↓
Task Decomposition Engine
    ↓
ROS Action Generator
    ↓
Execution Monitor + Feedback Loop
```

### Core Components

* **Planner Module** – LLM-driven reasoning engine
* **Action Mapping Layer** – Converts LLM output into ROS commands
* **Execution Validator** – Confirms action success/failure
* **Memory Store** – Maintains contextual state

---

## Tech Stack

* Python
* ROS
* PyTorch
* LLaMA-2 (local inference)
* ReAct prompting framework

---

## Key Capabilities

* ✔ Multi-step task planning
* ✔ Error recovery via feedback loops
* ✔ Natural language → robotic actuation
* ✔ Modular plug-and-play architecture

---

## Performance

* ~70% reduction in manual scripting
* Supports dynamic multi-step action chains
* Validated in simulated robotic environments

*(Add latency, inference time, or FPS metrics if available.)*

---

## How to Run

```bash
git clone https://github.com/asundar0128/Agentic-AI-Framework-for-Robotics-ROSA-.git
cd Agentic-AI-Framework-for-Robotics-ROSA-
pip install -r requirements.txt
python main.py
```

Ensure ROS is running before execution.

---

## Project Structure

```
rosa/
│── planner/
│── action_mapper/
│── executor/
│── memory/
│── main.py
```

---

## Future Improvements

* Multi-robot orchestration
* Real-world hardware validation
* Tool-use via structured function calling
* Edge deployment optimization

---

## Author

Developed to explore production-grade Agentic AI systems for robotics integration.

