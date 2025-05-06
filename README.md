# A2A Echo Agent

A simple echo agent implementation using Google's Agent-to-Agent (A2A) framework.

## Overview

This project demonstrates how to build an agent that can participate in the A2A ecosystem. The agent exposes a simple "Echo Tool" skill that reflects back any text input received.

The Echo Agent implements:

- Basic A2A server functionality
- Text input/output support
- Streaming response capability
- In-memory task management

## Prerequisites

- Python 3.13 or higher
- Git

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/A2A.git
cd A2A
```

2. Create a virtual environment and install dependencies:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -e .
```

## Usage

Start the server locally:

```bash
my-project --host localhost --port 10002
```

The Echo Agent will start running and listening for requests at http://localhost:10002/.

## Project Structure

- `src/my_project/__init__.py` - Main entry point and server initialization
- `src/my_project/task_manager.py` - Implementation of the Echo task manager
- `src/my_project/agent.py` - Agent configuration

## A2A Integration

This agent implements the Google A2A framework, which facilitates communication between AI agents. It registers itself with capabilities and skills so that other agents can discover and utilize it.

### Registered Skills

- **Echo Tool**: Echoes back any text input provided to it

### Capabilities

- **Streaming**: Supports streaming responses

## Development

To modify the agent's behavior, you can edit the `task_manager.py` file to implement different response logic.

## License

[Add appropriate license information here]

## Acknowledgments

- Google A2A Framework
