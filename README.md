# USRKey — your context, in six files

**Stop re-explaining yourself to every AI tool.** Fill in six short markdown
files about yourself, once. Hand the right ones to each tool. Works with every
AI assistant on the planet today — no install, no account, no integration.

> You told Claude your stack on Tuesday. On Wednesday, Cursor doesn't know.
> Thursday, another model asks again. Every AI tool keeps its own memory of
> you, or none. These six files are the fix you can do in ten minutes.

## The six pages

| File | What you put in it | How often it changes |
|---|---|---|
| [`identity.md`](identity.md) | Who you are — name, role, languages, timezone | Rarely |
| [`stack.md`](stack.md) | Your world — tools, environment, how you like to work | Every few months |
| [`now.md`](now.md) | What's true *this week* — current focus, situation | Weekly |
| [`history.md`](history.md) | Facts worth keeping — decisions, milestones | When something matters |
| [`boundaries.md`](boundaries.md) | How to treat you — what never to infer, store, or ask | Stable |
| [`agents.md`](agents.md) | Your tools, and what each one gets to see | When you add a tool |

**The rule that makes this safe: nothing goes in a page unless you chose to
write it.** Consent by authorship. Share `stack.md` with your coding tools and
keep `history.md` to yourself — each file is a boundary.

## Use it in ten minutes

1. **Use this template** (button above) or just copy the six files anywhere.
2. Fill in what you're comfortable sharing. Delete what doesn't apply.
3. Hand pages to tools — see [HOW-TO-USE.md](HOW-TO-USE.md) for the exact moves
   per tool (Claude, Cursor, ChatGPT, Cline, Continue, anything else).

The simplest move that works everywhere: paste the relevant pages at the top of
a conversation. The fancier moves (auto-loaded context files, MCP) are in the
how-to.

## What this template is — and isn't

This is **Level 0** of the [USRKey format](https://github.com/frank-bot07/usrcp/blob/main/spec/USRKEY-FORMAT.md):
plain files, maximum portability, zero infrastructure. It is deliberately
copyable — fork it, adapt it, translate it.

What plain files **don't** give you: encryption at rest, per-tool scope
*enforcement* (here a tool reads whatever file you hand it), an audit trail of
which tool saw or proposed what, sync across devices without trusting a server,
and writeback-by-proposal (tools suggesting updates to your pages that you
approve as diffs).

That's **Level 2 — the vault**: [USRCP](https://github.com/frank-bot07/usrcp),
the open-source reference implementation where these same six pages live in an
AES-256-GCM encrypted ledger under a key only you hold. Start with the files;
graduate to the vault when the files start mattering.

*Your context is yours. Carry the key.* — [the manifesto](https://github.com/frank-bot07/usrcp/blob/main/MANIFESTO.md)

## License

[CC0 1.0](LICENSE) — public domain. The format spreading is the point.
