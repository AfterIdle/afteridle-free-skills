# AfterIdle Starter (free)

One task in → 3–5 small steps for **today**, matched to your energy, with a safe place to stop. Works for any kind of work: writing, admin, study, chores, creative, client work, code.

## Quick start
- "Help me start my tax paperwork. Low energy."
- "Break down writing my newsletter for today, 20-min blocks."
- "Plan fixing the contact form. High energy."
- "I'm fading" (mid-plan) → it shrinks to the nearest safe stop.

## Install

The skill is one folder with a `SKILL.md`. Install the `afteridle-starter` folder (or `afteridle-starter.zip` from the Gumroad download).

- **Claude.ai / Claude apps:** Settings → Capabilities → Skills → upload the skill's ZIP (the folder is at the ZIP root).
- **Claude Code:** copy the folder to `~/.claude/skills/` (all projects) or `.claude/skills/` (one project).
- **Cursor:** copy the folder to `~/.cursor/skills/` (all projects) or `.cursor/skills/` (one project).

These paths come from each tool's docs at the time of writing. If your version differs, check its skills docs.

## Make it yours (preferences)

1. **Copy `afteridle-preferences.md` to your project root**, or paste its lines into `CLAUDE.md` or a Cursor rule. It's also inside the ZIP.
2. Delete keys you don't need and edit the rest. Missing keys use each skill's defaults.
3. **Precedence:** what you say in chat > the preferences file > the skill's defaults. "Just 10-minute steps today" beats the file.

| Key | Means |
|---|---|
| `tone`, `output_format`, `max_questions`, `resume_note` | All skills: voice, layout (checklist, table, Notion- or GitHub-ready), the most questions it asks before acting, and a "pick up here" line |
| `energy_scale`, `ask_energy_first`, `block_length`, `rest_between_blocks`, `task_order`, `max_blocks_per_day`, `planning_horizon`, `low_energy_tasks`, `max_steps` | Energy: how you rate energy, block and rest length, task order (auto: a quick win first when energy is low, hardest first otherwise; or easy-first / hard-first), daily cap, session/day/week, easy tasks for low days |
| `work_types`, `stack`, `audience`, `brand_voice`, `platforms` | Your work: what you do, your tools, who it's for, your voice, where you work |

Other keys in the file are used by paid AfterIdle kits; the Starter safely ignores them.

## Energy-aware by design

Small steps, a safe stopping point, and a resume line, so a low-energy day or a break never loses progress. Say "low energy" or "I'm fading" in any skill to get a smaller version. Stopping is never framed as failure.

**Need more?** Multi-day plans, several tasks, deadlines, and rest built in are in **Energy-Aware Planner** ($9, part of the Start & Focus Kit). Stopping mid-task? The free **Context Handoff** skill saves your place so you can resume in under 2 minutes. The Starter is complete on its own. Both at afteridle.gumroad.com.

---
AfterIdle · energy-aware skills for people who work in bursts with real rest · afteridle.gumroad.com
