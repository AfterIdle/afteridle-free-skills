# AfterIdle Free Skills

Two free, energy-aware Agent Skills for Claude (Claude.ai, Claude Code) and any agent that reads `SKILL.md`. Built for solo workers and neurodivergent-friendly productivity: small steps, real energy, clean stopping points.

| Skill | What it does |
|---|---|
| [`afteridle-starter`](skills/afteridle-starter) | Turns one task into 3 to 5 small steps for today, sized to the energy you have right now, with a safe place to stop. |
| [`context-handoff`](skills/context-handoff) | Saves exactly where you stopped (goal, state, the exact next action, gotchas) and gets you back in under 2 minutes. Also works for handing work to another chat, agent, or person. |

Works for any kind of work: writing, admin, study, client work, creative projects, code.

## Install

**Claude.ai:** download the ZIP for a skill from its Gumroad page (links below) and upload it under Settings, then Capabilities, then Skills.

**Claude Code:** copy a skill folder into `~/.claude/skills/` (or your project's `.claude/skills/`). Or add this repo as a plugin marketplace:

```
/plugin marketplace add AfterIdle/afteridle-free-skills
/plugin install afteridle-free-skills@afteridle
```

**Any other chat:** paste the `SKILL.md` and say "Follow these instructions for this conversation."

Each skill reads an optional `afteridle-preferences.md` so you can change step counts, tone, and stop rules.

## Get them on Gumroad (free)

- [AfterIdle Starter](https://afteridle.gumroad.com/l/afteridle-starter)
- [Context Handoff](https://afteridle.gumroad.com/l/context-handoff)

## Want more?

- [Start & Focus Kit](https://afteridle.gumroad.com/l/start-focus-kit) ($29): six skills for getting started and staying focused (Just Start Helper, Focus Session Designer, Idea Capture & Prioritizer, Voice Note to Action, Energy-Aware Planner, Weekly Reset).
- [Solo Dev Kit](https://afteridle.gumroad.com/l/solo-dev-kit) ($39): nine skills for solo developers, from project kickoff to debugging and refactoring.

Made by AfterIdle.

## License

Repository documentation and packaging are [MIT](LICENSE), copyright AfterIdle. The skills themselves (`skills/afteridle-starter` and `skills/context-handoff`) are for personal or single-business use and may not be resold or redistributed — the same terms as the free [AfterIdle Starter](https://afteridle.gumroad.com/l/afteridle-starter) and [Context Handoff](https://afteridle.gumroad.com/l/context-handoff) downloads.
