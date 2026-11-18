# agentdevelopmentkit

Google Agent Development Kit (ADK) sample project.

## Agent

- `agent.py` — defines `root_agent` (`gemini-flash-latest`) with a `get_current_time` tool.
- `multi_tool_agent/` — placeholder package for additional multi-tool agents.

## Run the ADK server

Prerequisites:
- Python 3.11+
- `pip install google-adk google-genai`
- Set `GOOGLE_API_KEY` in a `.env` file at the project root (not committed).

Start the ADK web server:

```bash
adk web
```

Or run the API server:

```bash
adk api_server
```

The server will load `root_agent` from `agent.py` and serve it via the ADK web UI / API.
