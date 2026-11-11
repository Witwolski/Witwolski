# Claude Lab — 7 nights, 7 things Claude can do

**When:** 7pm Brisbane time, Mon 9 Nov to Sun 15 Nov 2026. A reminder arrives in your Claude chat at 6:58pm each night.
**Where:** your phone, in the Claude app. Nothing here needs your home PC.
**Length:** 60 minutes. Tonight is shorter (30 min) because you've just flown in.

## RESET — this swing runs Night 4 and Night 5 only
Mon–Wed didn't happen. For the rest of this swing, only the two nights with deadlines are on:
- **Thu 12 Nov:** Night 4, money dashboard (payday).
- **Fri 13 Nov:** Night 5, Japan research (book by 30 Nov).

Nights 1, 2, 3, 6 and 7 move to the next swing. Each session is 30 minutes.

## Why this plan, and not "learn Claude"
You already use more of Claude than most people do: scheduled tasks, your own skills (payday, spending log, mortgage review), a tracker page with a database, Gmail emails, and browser scraping for fares.

Three big things are missing:
1. **Your actual job.** You work on PLC and SCADA upgrades, but none of your Claude projects touch that work.
2. **Building real software.** That means tests, pull requests and code review, not just prompts.
3. **Pages that think.** Your tracker stores data. It doesn't ask Claude anything.

Each night covers one area. You leave with **something you keep**, not just a demo.

## One rule for work nights
**Never paste client or employer files into your personal Claude account.** That includes PLC code, drawings, IO lists and site documents. Every work example in this plan uses a made-up plant. If you want to use real work data, check your company's AI policy first.

---

## The 7 nights

### Night 1 — Mon 9 Nov · Claude can see *(30 min, phone only)*
**What it is:** you can send Claude a photo or screenshot, and it reads it like text.
**Do:**
1. Take a photo of your mess dinner. Send it with: *"Score this against my plate rule: half veg, quarter protein, quarter carbs. Be blunt."*
2. Screenshot anything confusing from today (a flight email, an app setting, a form) and ask Claude to explain it.
3. Reply to the 7pm message with your Day 1 fitness test numbers.

Check your site's photo rules first. Many sites don't allow photos outside your room or the mess.
**Keep:** a habit of sending a photo to Claude instead of typing a description.

### Night 2 — Tue 10 Nov · A page that thinks
**What it is:** a page that works like a small app. It saves what you enter, and it can ask Claude questions by itself.
**Build:** a **Camp Food Scorer** for your phone. You type your meal (or snap it). The page asks Claude to score it against your six food rules and saves it to a log. It shows your score for the week.
**Do:** describe what you want in plain words, use it straight away, then ask for two changes.
**Keep:** the page, for every swing.

### Night 3 — Wed 11 Nov · Claude at work (made-up plant)
**What it is:** Claude can write engineering documents, PLC code and spreadsheets.
**The plant:** a pump station with two pumps in duty/standby (one runs, one waits as backup), one level transmitter, and high and low level alarms.
**Ask Claude for:**
1. A one-page functional description (what the system must do, in plain words).
2. IEC 61131-3 Structured Text (the text-based PLC language) for the duty/standby logic. It should swap the duty pump every 24 hours and change over to the standby pump on a fault.
3. A test sheet to check that logic.
4. An IO list as an Excel file (`.xlsx`).
5. Then: *"Find three bugs or edge cases in the code you just wrote."*

**Keep:** an honest view of where Claude saves you hours and where you'd never trust it without checking.

### Night 4 — Thu 12 Nov · Your money as a dashboard *(payday)*
**What it is:** Claude can read your tracker's data and turn it into charts you can tap on.
**Before:** your payday checklist arrives at 6:54am. Do the transfers.
**Build:** a dashboard page from your spending tracker. It shows:
- spending by category against your budget
- site weeks against home weeks
- your mortgage payoff timeline with and without the $200/week after-tax super payment

**Also:** give Claude the figures from your first FIFO payslip. Your 15 Nov spending review needs them.
**Keep:** a dashboard you can open on any payday.

### Night 5 — Fri 13 Nov · Deep research with a team of agents
**What it is:** Claude can hand parts of a big question to several helper agents. They search at the same time, and Claude writes a report with sources.
**Ask:** a 2-week Japan itinerary for February 2027 that works with your fare tracker's routes (Tokyo or Osaka). Cover snow areas, rail passes against single tickets, a daily cost in AUD, and what to book first.
**Why now:** your fare playbook says book by **30 Nov**.
**Keep:** a shareable doc you can send to whoever's going with you.

### Night 6 — Sat 14 Nov · Build software the professional way
**What it is:** Claude Code can plan, write code, write tests, open a pull request (a proposed change you review before it goes in) and review its own work.
**Build:** `tagcheck`, a small Python tool. It reads a PLC tag list (CSV) and flags tag names that break a naming rule, like `AREA_EQUIP_SIGNAL`. Use Night 3's IO list as the test data.
**The order:**
1. Plan mode first. Claude plans, you approve.
2. Build it, with tests.
3. Open a pull request.
4. Run `/code-review` on it.
5. Ask Claude to watch the pull request.

**Keep:** a pattern you can reuse for any tool you want at work.

### Night 7 — Sun 15 Nov · Claude that runs without you
**What it is:** scheduled tasks and automations that work while you sleep.
**Do:**
1. **Tidy up (15 min).** You have 10 scheduled tasks. Only 4 are on, and two are both called "Daily control systems test". Delete the dead ones.
2. **Build one new automation (30 min).** Idea: a **Sunday night weekly review email** that covers spending, Japan fares, fitness and food scores in one dashboard. It replaces several separate check-ins.
3. **Retro (15 min).** Fill in the scorecard in `LOG.md`.

**Keep:** fewer automations, and ones you actually read.

### Mon 16 Nov — fly home. No session.

---

## Home week: needs your PC, not your phone
These need a computer, so save them for home:
- **Computer use / Cowork:** Claude controls apps on your Windows PC, for example to sort files or fill in a form.
- **Claude in Chrome:** Claude uses websites in your own browser, while you're logged in.
- **Writing style profile:** Claude learns how you write from your sent emails, then drafts posts that sound like you. Pair it with your industry post ideas.
- **Claude API:** a Python script on your PC that calls Claude directly. It needs a separate API key and is billed separately.
- **Your budget spreadsheet:** have Claude update `Freedom_Budget.xlsx` directly.
