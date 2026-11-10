# Context Handoff (free)

Stop mid-task without losing the thread. It saves a short, exact note: the goal, where things stand, the last thing done, the **exact next action**, open questions, files and links, and gotchas. Later, "where was I?" gets you moving again in under 2 minutes. Works for any kind of work: code, writing, study, client work, admin, creative.

## Quick start
- "I need to stop. Save my place." (low energy: you get 2 lines, no questions)
- "Write a handoff I can paste into a new chat."
- "Switching to the client project. Save this one first."
- "Where was I?" or paste an old handoff, and it resumes.

## Install
Install `context-handoff.zip`, or the `context-handoff` folder (keep `references/` beside `SKILL.md`).
- **Claude.ai / Claude apps:** Settings → Capabilities → Skills → upload the ZIP.
- **Claude Code:** copy the folder to `~/.claude/skills/` or `.claude/skills/`.
- **Cursor:** copy the folder to `~/.cursor/skills/` or `.cursor/skills/`.
- **No skills support?** Paste `SKILL.md` into any chat and add "Follow these instructions for this conversation."

## Make it yours
Copy `afteridle-preferences.md` to your project root (or paste the lines into CLAUDE.md or a Cursor rule). Saying it in chat always wins.

| Key | Means |
|---|---|
| `handoff_length` | short (2 lines) / standard / full |
| `handoff_audience` | me / ai / person, the reader of the handoff |
| `save_to_file` | a file to append handoffs to, e.g. `HANDOFF.md` |
| `stale_after` | after this long, resume starts with a 2-minute "what changed" check |
| `energy_scale`, `block_length`, `resume_note`, `max_questions`, `tone`, `output_format` | shared with every AfterIdle skill |

## Safe by design
It never copies passwords, keys, tokens, or card numbers into a handoff. It points to where they live instead. It never claims progress that didn't happen, and guesses are marked.

**Pairs well with:** the free **AfterIdle Starter** (plan one task today), **Energy-Aware Planner** (days and weeks), and **Weekly Reset** (a kind look back). Together they're in the **Start & Focus Kit**.

afteridle.gumroad.com
