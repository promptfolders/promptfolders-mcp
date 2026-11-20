# PromptFolders MCP

Git-style version control for your prompts, readable by your AI through MCP.

PromptFolders keeps your prompts in one library with full version history, team spaces and review-before-merge. Connect it to Claude, Cursor or any MCP client and use your prompts right inside the chat.

- Website: https://promptfolders.com
- MCP endpoint: `https://promptfolders.com/mcp` (Streamable HTTP, OAuth 2.1)

## Tools

| Tool | What it does |
|---|---|
| `list_my_accessible_prompts` | Search the prompts you can access |
| `get_and_fill_prompt` | Fetch a prompt and fill in its variables |
| `create_prompt_from_chat` | Save a new prompt from the conversation |
| `save_prompt_version_from_chat` | Save a new version of an existing prompt |
| `duplicate_or_move_prompt` | Copy or move a prompt between spaces |
| `list_pending_proposals` | See team edits waiting for review |
| `review_proposal` | Approve or reject a proposed edit |
| `comment_on_proposal` | Comment on a proposed edit |

## Connect

**Claude (web / desktop):** Settings → Connectors → Add custom connector → paste `https://promptfolders.com/mcp` → sign in.

**Claude Code:**

```bash
claude mcp add --transport http promptfolders https://promptfolders.com/mcp
```

**Cursor** (`~/.cursor/mcp.json`):

```json
{
  "mcpServers": {
    "promptfolders": { "url": "https://promptfolders.com/mcp" }
  }
}
```

You sign in with your PromptFolders account the first time (OAuth). No API key needed.

## Links

- Privacy policy: https://promptfolders.com/privacy
- Support: support@promptfolders.com

This repository holds listing metadata only. The service is hosted at promptfolders.com.
