# Context Handoff: worked examples

Each example shows the request, then the output. The examples follow SKILL.md exactly.

## 1. Coding, mid-debug (standard, for me)

**Request:** "I need to stop. Save where I am on the logout bug." (In the chat: users get logged out after about 20 minutes; the token refresh in `src/auth/session.ts` was suspected; the clock skew theory was ruled out; `.env` has `JWT_SECRET=...`.)

```
## Handoff: Random logout bug   (Nov 3, energy at stop: medium)
Goal: users stay logged in; refresh works past 20 minutes.
State:
- Reproduces every time: log in, wait 20 min, click any link.
- Current hypothesis: refreshToken() in src/auth/session.ts never runs, because the timer starts before the token is saved (guess).
Last done: ruled out clock skew (server and client times match).
Next action: add a console.log at the top of refreshToken() in src/auth/session.ts:41, then run the 20-min repro once ← start here
Open questions: does the mobile app share this session code?
Files & links: src/auth/session.ts, src/auth/timer.ts, repro steps above
Gotchas: shorten the token life to 1 min in .env.local to test faster, and remember to set it back. The JWT secret lives in .env as JWT_SECRET (not copied here).
Can wait: the "remember me" checkbox styling.
Pick up next time: the log line in refreshToken().
```
Note to the user: "I left the JWT secret out of the handoff and pointed to where it lives."

## 2. Client / admin task (standard, for a person)

**Request:** "Write a handoff for my VA so she can finish the invoice chase while I'm out."

```
## Handoff: Overdue invoices chase   (Nov 3)
Goal: all 3 overdue invoices paid or with a promised date by Friday.
State:
- Café Lune (#1042, $650): reminder sent Oct 30, no reply.
- Hartley Studio (#1039, $1,200): they said "paying this week" on Nov 1.
- Pine & Co (#1045, $400): not chased yet.
Last done: sent the Café Lune reminder.
Next action (Maya): send Pine & Co the friendly reminder from the "Invoice reminder 1" template in Gmail, today ← start here
Open questions: if Café Lune doesn't reply by Wed, call or email? (I prefer email.)
Files & links: Invoices sheet (Drive > Admin > Invoices 2026), Gmail templates
Gotchas: Hartley pays by bank transfer, so it won't show in Stripe; check the bank feed instead.
Can wait: the new rates email to old clients.
Pick up next time: Pine & Co reminder.
```

## 3. Study / creative (short, low energy)

**Request:** "Fading. Save my place on the chapter 4 essay, no questions."

```
Handoff Nov 3: Ch. 4 essay (history). Last: outline done, intro paragraph drafted in essay-ch4.docx.
Next: write the first sentence of body paragraph 1 using the quote on p. 112 (~10 min)
```

## 4. Handing off to a fresh AI chat (ai)

**Request:** "This chat is getting long. Write a handoff I can paste into a new Claude chat to keep working on my Etsy listing copy."

```
Context for a fresh assistant: I sell printable planners on Etsy. We are rewriting the listing for the "Calm Week Planner" to be clearer and more search-friendly. Keep my voice: warm, plain, no hype, no "game-changer". Done = title (under 140 characters), first 2 lines of the description, and 13 tags.
## Handoff: Calm Week Planner listing   (Nov 3)
Goal: final title, opening 2 lines, 13 tags.
State:
- Title chosen: "Calm Weekly Planner Printable, Low Energy Planner, Undated A4/Letter".
- Opening lines (draft 2, the favorite): "A gentle weekly planner for low-energy weeks. One page, three priorities, and room to rest."
Last done: picked the title.
Next action: write 13 tags from the attached keyword list, each under 20 characters ← start here
Attach with this note: keywords.txt (the keyword list from eRank)
Don't: change the title, or mention ADHD as a diagnosis.
Pick up next time: the 13 tags.
```

## 5. Resume from a stale handoff (2 weeks old)

**Request:** pastes example 1, dated Oct 20. "Where was I? Low energy."

```
## Resume: Random logout bug   (handoff from Oct 20, 2 weeks old)
Goal: users stay logged in past 20 minutes.
You were: testing whether refreshToken() ever runs.
Check first (~2 min): git log since Oct 20 for src/auth/ — did anyone touch session.ts?
First action: add the console.log in refreshToken() and run the shortened 1-min repro (~10 min) ← start here
Then: if it never logs, look at where the timer starts in timer.ts.
```
Pick up next time: the result of the log line.

## 6. Switching projects (two short handoffs)

**Request:** "Switching from the newsletter to the client logo. Save both."

```
Handoff Nov 3: Newsletter #14. Last: wrote the main story. Next: pick the subject line from the 3 options at the top of newsletter-14.md (~5 min)
Handoff Nov 3: Café Lune logo. Last: 3 sketches scanned. Next: vectorize sketch B in logo.ai, outline only (~30 min) ← active now
```
