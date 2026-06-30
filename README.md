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

## Install (local marketplace)

```bash
claude plugin marketplace add ~/Projects/thinking-hats
claude plugin install thinking-hats@thinking-hats
```

Then in any session: `/black-hat`, `/hats`, etc. (names autocomplete after `/`).

## License

Personal project by Andrei Surdu.
