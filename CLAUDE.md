# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Python project for implementing a basic AI agent from scratch using UV as the package manager. The project explores fundamental agent concepts including architecture, decision-making, environment interaction, and learning capabilities.

## Development Commands

### Project Setup
- `uv sync` - Install dependencies
- `uv add <package>` - Add new dependencies

### Running the Project
- `uv run python src/construct_agent_from_scratch/main.py` - Run the main agent

### Development Tools
- `uv run pytest` - Run tests
- `uv run ruff format` - Format code
- `uv run ruff check` - Lint code
- `uv run ruff check --fix` - Auto-fix linting issues

## Project Structure

The project follows a standard Python package structure:

```
src/construct_agent_from_scratch/
├── __init__.py
├── main.py              # Main entry point
├── agent/               # Agent implementation modules
│   ├── __init__.py
│   └── base_agent.py
└── environment/         # Environment interaction modules
    ├── __init__.py
    └── base_environment.py
```

## Key Architecture Concepts

- **Agent Module**: Contains the core agent implementation and behavior logic
- **Environment Module**: Handles environment interaction and state management
- **Main Entry Point**: `src/construct_agent_from_scratch/main.py` serves as the primary execution point

## Development Guidelines

- Use UV for all dependency management
- Follow Python 3.10+ standards
- Run linting and formatting before commits
- Place agent-specific logic in the `agent/` module
- Place environment-related code in the `environment/` module