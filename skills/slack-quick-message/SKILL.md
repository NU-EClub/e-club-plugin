---
description: Send a quick message to a Slack channel
allowed-tools: mcp__plugin_e-club_slack__*
---

# Send Slack Message

Send a message to a Slack channel from Claude Code.

**Usage:** `/e-club:slack-quick-message #general Hey team, meeting moved to 3pm!`

## Instructions

1. Parse `$ARGUMENTS` to extract the channel name (starts with #) and the message text
2. Use the Slack MCP server to send the message to the specified channel
3. Confirm the message was posted successfully
