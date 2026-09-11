---
description: Create a task in the club's Notion tasks database from a natural-language description
allowed-tools: mcp__plugin_e-club_notion__*
---

# Create Notion Task

Create a new task in the E-Club Notion tasks database.

**Usage:** `/e-club:notion-quick-task Buy snacks for the next meeting`

## Instructions

1. Take the task description from `$ARGUMENTS`
2. Use the Notion MCP server to find the "Tasks" database
3. Create a new page in that database with:
   - Title set to the task description
   - Status set to "To Do"
4. Confirm the task was created and share the page link
