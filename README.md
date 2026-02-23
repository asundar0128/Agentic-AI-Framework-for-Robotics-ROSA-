# ROSA – Agentic AI Framework for Robotics

> Production-ready Agentic AI system that translates natural language instructions into executable ROS actions using ReAct reasoning and LLM planning.

## Overview

ROSA (Robotic Orchestrated Semantic Agent) connects Large Language Models with robotic control systems to enable:

- Natural language command interpretation
- Multi-step task decomposition
- Autonomous reasoning (ReAct framework)
- Structured ROS action generation
- Real-time execution validation and recovery

<img width="983" height="441" alt="ROSA_Architecture" src="https://github.com/user-attachments/assets/bb4e7e1f-1d0d-43b2-b271-8fa555ed62b8" />

ROSA demonstrates how Agentic AI can operate in robotics environments with dynamic planning and feedback loops.

## What It Does

ROSA converts a high-level instruction like:

"Pick up the red object and place it on the table"

Into actionable steps:

1. Locate red object  
2. Move to object  
3. Execute grasp action  
4. Navigate to table  
5. Release object  

## Human-Agent Interaction

ROSA is designed to be conversational. Unlike traditional robotics which require rigid code, ROSA handles:   

Clarification Dialogues: If a command is ambiguous (e.g., "Pick up the box" when there are two boxes), the agent will ask the user for clarification before acting.

Status Updates: The agent provides natural language feedback on its "Reasoning" process, explaining why it is choosing a specific ROS action.

Human-in-the-loop (HITL): Users can interrupt or modify plans mid-execution through the dialogue interface.

Then translates this into executable ROS action calls.

<img width="562" height="644" alt="rosa" src="https://github.com/user-attachments/assets/136fde47-96d1-4259-84be-05c6fdeaff43" />

## Environment Variables & Setup

ROSA requires the following environment variables:

```bash
ROS_MASTER_URI=http://localhost:11311
ROS_HOSTNAME=localhost
OPENAI_API_KEY=your_openai_api_key_here
```

## Dependencies

- Python 3.10+
- ROS Noetic / ROS2 (depending on your setup)
- Python packages in requirements.txt
- Docker (optional, for containerized deployment)

## Quickstart

# Clone the repository
git clone https://github.com/asundar0128/Agentic-AI-Framework-for-Robotics-ROSA-.git
cd Agentic-AI-Framework-for-Robotics-ROSA-

# Configure environment
cp .env.example .env

# Install Python dependencies
pip install -r requirements.txt

# Start ROS master (if not using Docker)
roscore

# Run ROSA
python run_rosa.py

# Optional: Docker deployment
docker compose up --build -d

## Key Capabilities

- Multi-step reasoning via ReAct
- LLM-driven task planning
- Structured ROS command mapping
- Execution monitoring + retry logic
- Context-aware memory store
- Modular, plug-and-play design

## System Architecture

![Robotics Framework](https://github.com/user-attachments/assets/7dce2fa0-842f-4a6b-bf76-0217755fd5d6)

## Tech Stack

- Python
- ROS
- PyTorch
- LLaMA-2 (local inference)
- ReAct prompting framework

## Performance

- ~70% reduction in manual scripting
- Supports dynamic multi-step action chains
- Validated in simulated robotic environments

## Project Structure

rosa/
│── planner/
│── action_mapper/
│── executor/
│── memory/
│── main.py

## Future Improvements

- Multi-robot orchestration for collaborative task execution
- Real-world hardware validation
- Tool-use via structured function calling

## Why This Project Matters

ROSA demonstrates:

- Agentic AI applied to real-world robotics
- LLM reasoning integrated with control systems
- Autonomous planning and execution
- Production-style modular design

This project showcases applied AI systems engineering beyond model training.

## Author

Built as a production-style Agentic AI robotics framework to demonstrate LLM-driven robotic orchestration.
