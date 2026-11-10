# AfterIdle preferences

Put this file in your project root, or paste the lines into CLAUDE.md or a Cursor rule. Every AfterIdle skill reads these exact keys. Delete what you don't need; anything missing uses the skill's default. Saying something in chat always wins.

## General (all skills)
```
tone:          calm, plain, no hype   # e.g. very brief / gentle / direct
output_format: as shown in Output format   # or checklist / table / plain text / Notion- or GitHub-ready
max_questions: 2   # most clarifying questions before acting
resume_note:   yes   # end with one line on where to pick up
```

## Energy (Starter, Planner)
```
energy_scale:        low / medium / high   # or 1-5, spoons, battery %, own words
ask_energy_first:    yes   # no = assume medium and say so
block_length:        15-45 min   # length of one step/block/increment
rest_between_blocks: 5-15 min   # or none
task_order:          auto   # auto / easy-first / hard-first; auto = low energy: quick easy win, then the hard one, then rest; medium/high: hardest first
max_blocks_per_day:  4
planning_horizon:    session   # session / day / week
low_energy_tasks:    sort, format, file, tidy, easy replies
max_steps:           5   # Starter: steps per session
```

## Handoffs (Context Handoff)
```
handoff_length:   standard   # short (2 lines) / standard / full
handoff_audience: me   # me / ai (another chat or agent) / person
stale_after:      3 days   # older handoffs get a "check what changed" step
save_to_file:     no   # e.g. HANDOFF.md
```

## Your work
```
work_types:   any   # e.g. client design + study + code
stack:        detect from project, else ask   # e.g. Next.js + Tailwind, Notion + Canva
audience:     solo neurodivergent builder   # who the work/output is for
brand_voice:  none   # e.g. warm, direct, no hype
platforms:    Gumroad   # where you sell/post: Etsy, Shopify, Instagram…
target_model: any   # Claude / Cursor agent / ChatGPT / other
domains:      dev, creative, general   # Prompt Upgrader template sets; general = anything else (business, personal, research)
```

## Code & design (Solo Dev Kit)
```
run_commands:          ask first   # ask first / allowed / never
tests:                 when a test setup exists   # always / when a test setup exists / never
accessibility:         WCAG 2.2 AA
design_system_source:  detect   # tokens file, Tailwind config, Storybook, or infer
research_depth:        quick   # Codebase Researcher: quick / standard / deep
save_to_file:          no   # path to save reports/notes, e.g. docs/NOTES.md
timebox:               30 min per hypothesis   # Debug Master
max_steps_per_session: 3   # Refactoring Expert
story_format:          user story   # user story / job story / plain task
max_phases:            4   # Project Launcher
```

## Business & ops (Launch Runner, Scope Keeper, Admin Triage, Weekly Reset, Repurposer)
```
launch_watch:       48h   # Launch Runner: how long the calm post-launch check runs
review_day:         end of week   # Weekly Reset: e.g. Friday afternoon / Sunday
top_priorities:     3   # Weekly Reset: priorities carried into next week
rate_bands:         ask   # Scope Keeper: your price ranges, e.g. small $300-600 / medium $800-1500
revisions_included: 2 rounds   # Scope Keeper: default revisions in a quote
channels:           ask   # Repurposer: e.g. X, LinkedIn, Bluesky, newsletter, Gumroad update
max_posts_per_week: 2   # Repurposer: posting cap so visibility doesn't eat build time
triage_batch:       25 min   # Admin Triage: length of one triage session
```
