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

## Getting started (Just Start Helper)
```
first_step_max:   2 min   # 30 sec / 1 min / 2 min / 5 min
start_options:    3   # 1-3 first-step options; low energy always gets 1
momentum_steps:   2   # follow-on steps after the first (0-3)
stop_after:       10 min   # or "first step only"
blocker_check:    yes   # name what's in the way in one line
body_doubling:    no   # yes = "tell me when it's done, I'll wait"
```

## Focus sessions (Focus Session Designer)
```
session_length:     auto   # auto (from energy) or e.g. 25 min / 50 min / 90 min
focus_rhythm:       auto   # auto / pomodoro (25+5) / 50-10 / one block
max_session:        90 min   # hard ceiling for one block
break_length:       5-10 min
body_checks:        yes   # water, food, movement at breaks
meds_reminder:      no   # yes = a "meds check" line at breaks (never names or doses)
hyperfocus_guard:   yes   # agreed hard stop + off-screen stop signal
interruptions:      note-and-return   # note-and-return / pause-and-resume / end-session
environment_prompt: yes   # one setup line
```

## Ideas (Idea Capture & Prioritizer)
```
max_priorities:    3   # ideas to act on; low energy always 1
scoring:           quick   # quick (pull / effort / fit) / none / own words
shiny_object_rule: park-and-return   # park-and-return / quick-look / ask-me
parking_lot:       here   # here / ideas.md / a tool you name
show_parked:       full   # full / grouped / count
keep_wording:      yes
review_cadence:    weekly
current_focus:     none   # e.g. "finish the course launch"
```

## Voice notes (Voice Note to Action)
```
max_actions:    7
next_step:      top-1   # top-1 / each / none
sections:       actions, decisions, questions, parked
show_quotes:    unclear-only   # unclear-only / none / all
filler_cleanup: yes
language:       match   # or a language you name
dates:          as-said   # as-said / ask / convert (only with today's date)
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
