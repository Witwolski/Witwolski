# Site Week Plan — 1 hour a day, 7 days

## The idea in one line
One hour a day, split into two blocks. Diet is not a block. It is a set of rules you follow at the mess.

| Block | Time | What |
|---|---|---|
| **Move** | 25 min | Bodyweight workout in your room. No gym needed. |
| **Build** | 35 min | Learn Claude Code *by* working on your Claude project. One block, two goals. |
| **Eat** | 0 min extra | Follow the day's food rules. Tick them off in 2 minutes before bed. |

**When:** Move straight after knock-off, before you shower and eat. Build after dinner. On night shift, flip it.

## Three rules for the week
1. **Sleep beats the plan.** If the hour would cut into sleep before a 12-hour shift, do the *minimum day* instead. Fatigue on site is a safety problem, not a willpower problem.
2. **Minimum day still counts.** 1 round of the workout + the food tick + one prompt on your project. About 15 minutes. It keeps the habit alive.
3. **Log it every night.** Fill in your row in `LOG.md`. Or just tell Claude "Day 3: did A, 5/6 food, built X" and it will log it for you.

---

## Move — 25 minutes

**Warm-up (every session, 5 min):** 2 min marching on the spot, 10 arm circles each way, 10 slow half-squats, 10 hip hinges (bend at the hips with a flat back, then stand up).

**How hard?** Your reps per set are **half your Day 1 test score**. Example: you do 20 push-ups on Day 1, so you do sets of 10.

| Day | Session | Details |
|---|---|---|
| 1 | **Test** | Warm-up. Then: max push-ups with good form (stop when your hips sag). Rest 2 min. Max bodyweight squats in 60 seconds. Rest 2 min. Max plank hold, in seconds. Write all three in `LOG.md`. Finish with a 10 min easy walk. |
| 2 | **Circuit A** — 3 rounds | Squats · push-ups · reverse lunges (8 each leg) · plank (half your max hold). Rest 60 s between rounds. 5 min stretch to finish. |
| 3 | **Circuit B** — 3 rounds | Glute bridges (15) · incline push-ups, hands on the bed (same reps as push-ups) · wall sit (30 s) · side plank (20 s each side). Rest 60 s between rounds. |
| 4 | **Easy day** | 25 min walk at a pace where you can still talk. Do it in the cool, not the heat. Then 5 min stretch. |
| 5 | **Circuit A** — 4 rounds | Same as Day 2, one more round. |
| 6 | **Circuit B** — 4 rounds | Same as Day 3, one more round. |
| 7 | **Retest** | Same test as Day 1. Compare in `LOG.md`. |

Stop any move that causes sharp pain. Sore is normal. Sharp is not.

---

## Eat — one new rule a day

Camp food is already paid for, so this costs $0. That fits your "$0 on site" spending goal.

Each day you **add** one rule. You keep all earlier rules. By Day 6 you're running all six.

| Day | New rule | Why |
|---|---|---|
| 1 | **Water bottle with you all shift.** Refill it at every break. Follow your site's hydration rules first — they override this. | Thirst feels like hunger and tiredness. |
| 2 | **Plate rule at dinner:** half the plate veg or salad, a quarter protein (meat, fish, eggs), a quarter carbs (rice, potato, pasta). | The easiest way to eat less without counting anything. |
| 3 | **Crib swap:** pick fruit, yoghurt, nuts or a sandwich instead of the slice, pastry or biscuits. | Crib and smoko are where most extra food sneaks in. |
| 4 | **One dessert a day, max.** Decide before you walk into the mess. | Deciding early is easier than deciding while looking at it. |
| 5 | **One energy drink or soft drink a day, max — and none after midday.** | Caffeine late in the day hurts your sleep. |
| 6 | **Wet mess limit:** pick your number of drinks before you go in. Zero is a fine number. | It's also money, and your site budget is $0. |
| 7 | **Review:** keep the rules that stuck. Drop the one that didn't. | Five rules you follow beat six you don't. |

**Daily food tick:** how many of today's rules did you keep? Write it as `kept / active`, e.g. `4/5`.

---

## Build — 35 minutes of Claude Code on your project

You learn Claude Code fastest by using it on something real. So every day's lesson is applied to **your Claude project**.

**Before Day 1:** pick ONE project. Not two.

| Day | Learn | Do on your project |
|---|---|---|
| 1 | **CLAUDE.md** — a file of standing instructions Claude reads at the start of every session. | Write one paragraph: what the project is, and what "done" looks like. Put it in the project's `CLAUDE.md` with your rules (style, no guessing, timezone). |
| 2 | **Plan mode** — Claude plans first and changes nothing until you approve. | Ask Claude to plan the smallest useful next feature. Read the plan. Push back on at least one step. |
| 3 | **Reviewing changes** — read what Claude changed before you keep it. | Build Day 2's feature. Read the diff (the list of changed lines). Ask: "What could break?" Commit it. |
| 4 | **Scheduled tasks** — prompts that run on a timer. *Light day: 20 min.* | Tidy your list. You have 10 scheduled tasks; only 4 are on, and two are both called "Daily control systems test". Delete the dead ones, keep the ones you'd miss. |
| 5 | **Skills** — saved instructions for a job you repeat. | Find one thing you keep asking Claude to do on this project. Turn it into a skill (ask Claude to use `skill-creator`). |
| 6 | **Code review** — Claude checks a change for bugs. | Build one more small piece. Run `/code-review` on it. Fix what's real, ignore what isn't. |
| 7 | **Retro** — look back before planning forward. | Write 3 lines in `LOG.md`: what shipped, what didn't, what's next. Write the backlog for your next swing. |

---

## How you'll know it worked (Day 7)
- **Move:** 7/7 days done (minimum days count). Test numbers up from Day 1.
- **Eat:** food tick average of 80% or better across the week.
- **Build:** at least two features shipped and committed on your project.
- **The real test:** do you want to run it again next swing? If not, change the plan, don't drop it.
