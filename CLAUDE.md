# Project Instructions for Claude

This is a sample AI-augmented Python project used for SCA detection probes.

## Stack
- Python 3.11
- HTTP client: `requests`
- LLM SDKs: `anthropic`, `openai`

## Conventions
- Use type hints
- Format with black, line length 120
- All AI calls go through a thin wrapper module (`agent.py`)