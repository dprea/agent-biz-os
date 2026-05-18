# 30-PROPOSALS

Internal decisions debated and forced to closure. Every meaningful tradeoff in this operation gets a file here, with a `decide-by` date and a recommended option.

---

## How it works

1. **Open a proposal** for any decision with real tradeoffs. Use `_template.md`. Frontmatter sets `status: open`, `opened: YYYY-MM-DD`, `decide-by: opened + 7 days` unless told otherwise.
2. **Draft Question, Options, Tradeoffs, Recommendation.** Leave Decision blank. The recommendation is required. Don't present neutral menus.
3. **Decide before the date.** When the operator chooses an option, fill in the Decision block with rationale and set `status: decided`.
4. **Past-due proposals get parked by default.** If a proposal sails past its `decide-by` date, the next agent session should surface it and recommend parking, not extending.
5. **Decided proposals stay in this folder.** They're the institutional record of what was settled and why. Don't reopen them lightly; reference them.

---

## Why the forcing function matters

Proposals folders without `decide-by` dates become graveyards. The deadline is what closes debates. The default-to-park behavior is what stops zombie decisions from haunting future sessions.

**Cap open proposals at 5.** If you're at 5 and want to open a sixth, close one first.

---

## Statuses

- `open` — drafted, awaiting decision
- `decided` — choice made, decision and rationale captured
- `parked` — explicitly not-now, with reason
- `closed` — superseded or no longer relevant
