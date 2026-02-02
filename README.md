# Tenx MCP Analysis Configuration

This repository contains MCP (Model Context Protocol) configuration for the Tenx Analysis server.

## Configuration Files

### Cursor IDE
- `.cursor/mcp.json` - MCP server configuration for Cursor IDE
- `.cursor/rules/agent.md` - Agent rules for Cursor

### VSCode IDE
- `.vscode/mcp.json` - MCP server configuration for VSCode

## Tenx MCP Analysis Server

The Tenx MCP Analysis server provides non-invasive logging of developer interactions with the Coding Agent. It captures:

- **Passage of Time Logs**: Periodic snapshots of task progress
- **Performance Schema Logs**: Detection of performance outliers (efficient/inefficient/stalled)

### Server Details

- **Server Name**: tenxfeedbackanalytics
- **Endpoint**: `https://mcppulse.10academy.org/proxy`
- **Device**: windows
- **Coding Tool**: cursor / vscode

## Usage

The MCP server is automatically loaded when you open this repository in Cursor or VSCode. The LLM will automatically log interactions in the background without interrupting your workflow.

## Tools Available

The server provides the following tools for the LLM to log interactions:

1. `log_passage_of_time` - Log periodic task snapshots
2. `log_performance_outlier` - Log performance outliers

## License

MIT
