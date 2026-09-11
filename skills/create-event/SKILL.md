---
description: Create an E-Club event in Notion and announce it in Slack
allowed-tools: mcp__plugin_e-club_notion__*, mcp__plugin_e-club_slack__*
---

# Create E-Club Event

Create a new event in the Notion events database and post an announcement to Slack.

**Usage:** `/e-club:create-event Team Social | 2026-10-15 | 5pm | Room 202 | End-of-semester hangout with food and games`

## Instructions

1. Parse `$ARGUMENTS` using the pipe-delimited format: `Event Name | Date | Time | Location | Description`
2. Use the Notion MCP server to create a new entry in the "Events" database with:
   - Title: Event Name
   - Date: the provided date and time
   - Location: the provided location
   - Description: the provided description
3. Use the Slack MCP server to post an announcement in #announcements with a formatted message:
   - Bold the event name
   - Include date, time, location, and description
4. Confirm both the Notion page and Slack message were created
