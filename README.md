# thinking-hats

Edward de Bono's **Six Thinking Hats** as Claude Code skills.

The method splits thinking into six modes and wears them **one at a time**, so facts,
feelings, caution, and optimism stop stepping on each other. A hat isn't a mood you argue
from — it's a direction you point all your attention at, on purpose, for a while.

Put on a single hat to focus the next reply through that one lens, or run `/hats` to take an
idea through the whole panel in one pass.

## The hats

| Skill | Hat | Lens |
|-------|-----|------|
| `/white-hat`  | ⚪ White  | Facts and data — what we know vs. assume, the numbers, the gaps |
| `/red-hat`    | 🔴 Red    | Gut feeling — a short emotional reaction, no justification |
| `/black-hat`  | ⚫ Black  | Caution — what could go wrong, weak points, failure modes |
| `/yellow-hat` | 🟡 Yellow | Optimism — benefits, value, best realistic case |
| `/green-hat`  | 🟢 Green  | Creativity — new ideas, alternatives, "what else" |
| `/blue-hat`   | 🔵 Blue   | Process — manage the thinking: what's open, which hat next |
| `/hats`       | 🎩 Panel  | Run all six over an idea, then a blue-hat synthesis |

## How a hat answers

Solo hats answer in **B → A → C** order — questions first, on purpose, so they prime your
own thinking before any answer biases it:

- **B — Questions first:** the sharp questions the lens raises.
- **A — The lens:** a short, plain prose pass speaking from that lens.
- **C — Takeaways:** a scannable bullet summary.

Two exceptions: **red** is gut-only (no questions, no reasons), and inside the **`/hats`
panel** each hat is compressed to A + C while the blue hat collects the open questions and
writes the close.

All seven skills share one source of truth for the lenses:
[`plugins/thinking-hats/hats/lens.md`](plugins/thinking-hats/hats/lens.md). Edit a lens
once and every skill follows.

## Examples

Same idea on the table for all three: **"add a daily-login streak reward to the game."**

### `/black-hat` — one lens, full B → A → C

> **B — Questions to sit with**
> - What happens to a player who misses day 6 of a 7-day streak — rewarded, or punished?
> - Are we rewarding *playing the game*, or just *opening the app*?
> - What stops a player who breaks a 200-day streak from quitting out of frustration?
>
> **A — The lens**
> A streak rewards *attendance*, not enjoyment, so you train players to show up out of
> obligation. The break is where it bites: a single missed day wipes a long streak, and loss
> aversion turns your most loyal players into your biggest flight risk…
>
> **C — Takeaways**
> - Rewards attendance, not fun — trains obligation · weight: high
> - Streak-break loss aversion = flight risk for your best players · weight: high
> - Invites bots, alts, open-and-close farming · weight: med

### `/red-hat` — gut only, no reasons

> Tired. It smells like a chore dressed up as a gift, and a little cynical — like we're
> nudging people instead of trusting the game to be worth opening.

### `/hats` — the full panel, compressed, blue closes

> ⚪ **White** — Strong prior art (Duolingo, Snapchat); missing our own day-7/30 retention
> baseline and a success metric.
> 🔴 **Red** — Tired. Smells like a chore dressed up as a gift.
> ⚫ **Black** — Streak-break loss aversion is a flight risk; rewards showing up, not playing.
> 🟡 **Yellow** — Habit is the highest-leverage retention lever; cheap to build and A/B test.
> 🟢 **Green** — Forgiving streak ("5 of 7 days"), reward *play* not the open, or a comeback
> bonus for returning after a lapse.
> 🔵 **Blue** — *Open:* is the problem login frequency or session depth? *Synthesis:* the goal
> is sound but the plain chain backfires; ship a forgiving, play-based variant and A/B it
> against control on retention lift, not streak vanity numbers.

## Install (local marketplace)

```bash
claude plugin marketplace add ~/Projects/thinking-hats
claude plugin install thinking-hats@thinking-hats
```

Then in any session: `/black-hat`, `/hats`, etc. (names autocomplete after `/`).

## Inspiration

This collection draws on the ideas, structure, and method of:

- **Edward de Bono** — _Six Thinking Hats_ (1985), the book this whole project is built on.

## Connect

Built by Razvan Andrei Surdu in Europe — [surdu.eu](https://surdu.eu) · [github.com/andreiRS](https://github.com/andreiRS)
