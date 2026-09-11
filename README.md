# E-Club Plugin for Claude Code

This plugin integrates Notion and Slack into Claude Code so you can manage tasks, send messages, and create events without leaving your AI assistant.

## What's Included

- **Notion Integration** - Create tasks, browse databases, manage pages
- **Slack Integration** - Send messages, post announcements
- **Pre-built Skills** - Quick workflows for common club operations

## Installation

### Step 1: Add the marketplace

```
/plugin marketplace add NU-EClub/e-club-plugin
```

### Step 2: Install the plugin

```
/plugin install e-club@NU-EClub-marketplace
```

Run `/reload-plugins` if prompted.

## One-Time Setup (OAuth)

After installing, you need to connect your Notion and Slack accounts:

1. Run `/mcp` in Claude Code
2. Click the **Notion** server and authenticate with your Notion account
3. Click the **Slack** server and authenticate with your Slack workspace
4. You're all set!

Tokens are cached so you only do this once.

## Skills

### Create a task

```
/e-club:notion-quick-task Buy snacks for the next meeting
```

### Send a Slack message

```
/e-club:slack-quick-message #general Hey team, meeting moved to 3pm!
```

### Create an event (Notion + Slack announcement)

```
/e-club:create-event Team Social | 2026-10-15 | 5pm | Room 202 | End-of-semester hangout
```

## Troubleshooting

**"Notion/Slack not authenticated"** - Run `/mcp` and complete the OAuth flow for the missing service.

**"Skill not found"** - Run `/reload-plugins` to refresh.

**"Tool not found"** - Run `/mcp` and verify both Notion and Slack show as connected.
