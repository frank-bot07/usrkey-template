# How to hand your pages to each tool

The principle everywhere: **give each tool only the pages listed for it in your
[`agents.md`](agents.md).** Three delivery moves, from zero-setup to fancy.

## Move 1: the paste card (works with literally everything)

Open the pages a tool is allowed, copy, paste at the top of the conversation
(or into the tool's "custom instructions" box). Done. Suggested wrapper:

```
<!-- usrkey:bundle for=chatgpt-web rendered=2026-06-11 -->
...paste identity.md...
...paste stack.md...
<!-- usrkey:end -->
```

Where the boxes live:
- **ChatGPT** → Settings → Personalization → Custom Instructions
- **Claude (web/desktop)** → Project instructions, or just paste in-chat
- **Gemini** → Saved Info
- Anything else → first message of the conversation

## Move 2: auto-loaded context files (coding tools)

Most coding assistants already slurp a context file from your home or project
directory. Concatenate the allowed pages into the file each tool reads:

| Tool | Where it reads context |
|---|---|
| Claude Code | `~/.claude/CLAUDE.md` (global) or `./CLAUDE.md` (project) |
| Cursor | `.cursorrules` or Settings → Rules for AI |
| Cline / Continue | their rules/instructions file or settings pane |
| Codex CLI | `AGENTS.md` in the repo |
| Aider | `CONVENTIONS.md` (via config) |

Tip: keep the six master files in one folder (e.g. `~/usrkey/`) and copy
*subsets* into each tool's file. The master is yours; tools get bundles.

Refresh rhythm: `now.md` weekly, the rest when they change.

## Move 3: the vault (encrypted, scoped, synced — one source of truth)

When manually copying bundles gets old, graduate to
[USRCP](https://github.com/frank-bot07/usrcp): the same six pages stored in an
AES-256-GCM encrypted local ledger under a key only you hold, served to tools
over MCP with your `agents.md` policy *enforced* (not honor-system), an audit
log of every access, and encrypted sync across your machines. Your pages, with
locks. See the [USRKey format spec](https://github.com/frank-bot07/usrcp/blob/main/spec/USRKEY-FORMAT.md)
for what "Level 2" guarantees.

## Two habits that make this work

1. **Update `now.md` weekly.** A stale now-page teaches tools to ignore you.
   Put it in your Monday routine.
2. **When a tool learns something about you worth keeping, *you* write it
   down** (in the right page) — don't let it live only in that tool's memory.
   That's the whole point.
