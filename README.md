# ADK Day Trip Planning Agent

A specialized AI agent built with Google's Agent Development Kit (ADK) that generates creative and fun day trip plans based on user preferences, location, and budget constraints. Built as part of **Gen AI Academy APAC - Cohort 2 (Student Track)**.

## Features

- 🎯 **Personalized Planning**: Generates trip suggestions based on user interests and preferences
- 📍 **Location-Aware**: Works with city names and GPS coordinates
- 💰 **Budget-Conscious**: Targets moderate budget activities (affordable yet valuable)
- 🔍 **Real-Time Search**: Uses Google Search to find current events and venues
- 📅 **Date-Specific**: Plans activities for specific weekend dates
- 🎨 **Creative Suggestions**: Maximum 3 distinct activities per plan with detailed location info
- 🤖 **Multiple Agent Types**: Single agent, sequential, parallel, loop, routing, memory, and MCP agents

## Project Structure

adk_tutorial-main/
├── a_single_agent/            # Basic single agent - Day Trip Planner
├── b1_sequential_agent/       # Sequential agent pipeline
├── b2_parallel_agent/         # Parallel agent execution
├── b3_loop_agent/             # Loop agent pattern
├── b4_manual_sequential_flow/ # Manual sequential flow
├── c_custom_agent/            # Custom agent implementation
├── d_routing_agent/           # Router agent pattern
├── e_agent_as_tool/           # Agent as tool pattern
├── f_agent_with_memory/       # Agent with memory
├── g_agents_mcp/              # MCP agents
└── mcp_tool_box/              # MCP toolbox

## Prerequisites

- Python 3.9 or higher
- Google AI Studio API key (free) — get yours at https://aistudio.google.com


## Quick Setup (Windows)

### Step 1: Download the repository
Open PowerShell and run:

Invoke-WebRequest -Uri "https://github.com/cuppibla/ADK_Basic/archive/refs/heads/main.zip" -OutFile "$HOME\ADK_Basic.zip"
Expand-Archive -Path "$HOME\ADK_Basic.zip" -DestinationPath "$HOME\ADK_Basic"
cd "$HOME\ADK_Basic\adk_tutorial-main"

### Step 2: Create virtual environment

python -m venv .adk_env
.adk_env\Scripts\Activate.ps1
pip install --upgrade pip
pip install -r requirements.txt

### Step 3: Create .env file

notepad a_single_agent\.env

Add these lines (replace with your actual API key):

GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=your_actual_api_key_here

## Running the Agent

### Activate virtual environment

cd "$HOME\ADK_Basic\adk_tutorial-main"
.adk_env\Scripts\Activate.ps1

### Run the ADK web interface

adk web

### Open in browser
Go to http://127.0.0.1:8000 → select a_single_agent from dropdown → start chatting!

### Example query
Plan me an affordable day trip to Tokyo for June 14-15, 2026.
Interests: outdoors, foodie, culture

## Deactivating the Environment

deactivate

## Cost
- Free — uses Google AI Studio free tier
- No Google Cloud billing account required
- No credit card needed

## Built With
- Google Agent Development Kit (ADK) — https://google.github.io/adk-docs/
- Gemini 2.5 Flash — https://aistudio.google.com
- Python 3.11

## Part of
Gen AI Academy APAC - Cohort 2
https://hack2skill.com/event/apac-genaiacademy