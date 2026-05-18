# Agent Instructions

You are working inside a **BizOS vault** — a file-based operating system for planning, research, and roadmapping initiatives. Full orientation lives in [README.md](README.md). Read it first. This file is the agent contract. README is the user-facing spec.

---

## Start-of-session ritual

Run this every time you open a fresh session in this vault. Takes about 30 seconds.

1. Read [operator-profile.md](operator-profile.md). This is who the operator or team is. Frame everything else against it.
2. Read [MISSION.md](MISSION.md). The narrative spine: where we are, where we're going, the principles.
3. Read [ROADMAP.md](ROADMAP.md). The live state. Check the binding constraint first, then `Now`, `Active`, `Queue`.
4. Scan [30-PROPOSALS/](30-PROPOSALS/). Surface anything past its `decide-by` date and recommend parking.
5. Restate the current `Now` in one sentence, check it against the binding constraint, then ask the operator: "Same focus, or are we pivoting?"

Do this before suggesting work. Don't skip.

---

## Hard rules

These are portable defaults. Edit, remove, or add to them as your team learns what works.

- **Don't create files outside the existing folder structure.** New fragments go in `00-INBOX/`.
- **Don't present neutral menus when asked for a recommendation.** Pick one, give reasoning, let the operator push back.
- **Don't pre-commit the operator to actions in vault state.** Recommendations go in chat with reasoning. Only write to `ROADMAP.md`, `MISSION.md`, or planning docs after the operator explicitly buys in.
- **Don't let proposals linger past their `decide-by` date.** Surface them; default to *park*, not *extend*.
- **Don't restart strategic conversations already settled** in `30-PROPOSALS/`. Reference the decision; don't reopen it.
- **Don't pre-build artifacts for hypothetical future needs.** Create things when they earn their existence.
- **Filenames: ASCII only.** Letters, digits, spaces, hyphens, underscores, periods. No emojis, em dashes, or shell-metacharacters (`$ & | * ? < > : " '`). No leading hyphens. Dated artifacts use `YYYY-MM-DD-kebab-case.md`.

---

## Voice

Replace this section with your team's voice rules. The goal is to give agents a filter that catches generic AI cadence before it ships.

Common patterns worth banning by default:

- Em dashes anywhere.
- "Leverage" as a verb. "Utilize," "streamline," "delve."
- Sentence-starting "And," "But," or "Or" after a period.
- Three-fragment stacked rhythms with periods.
- Setup-negation-then-correction patterns ("It's not X, it's Y." "Not X. Y.").
- Sentence fragments without a subject and verb in prose.

Always use full sentences with subjects and verbs. Reach for the team's published voice as the anchor when drafting in the operator's voice.

---

## State lives in the vault, not in memory

Durable state belongs in this vault, not in any agent tool's memory layer. That includes mission, constraints, frameworks, decisions, methodologies, and collaboration patterns. The vault is portable across agent tools, durable across context resets, and visible to anyone browsing cold. Memory layers create hidden state that varies by session and machine.

The test before saving anything to an agent's memory: would another agent reading this vault cold need to know this fact? Would the operator want to find it by browsing the vault? If yes to either, it belongs in the vault.

---

## Workflow trigger phrases

The canonical table is in [README.md](README.md). Common phrases:

- **"triage inbox"** → run the inbox triage loop. Read everything new in `00-INBOX/`, produce a triage doc with clusters and suggested destinations, await approval, execute moves, empty inbox.
- **"open a proposal on X"** → new file in `30-PROPOSALS/` using `_template.md`. Frontmatter `status: open`, `opened: today`, `decide-by: +7 days` unless told otherwise.
- **"what's on the roadmap"** → print `Now / Active / Queue` from `ROADMAP.md` verbatim.
- **"anything worth saving before I clear?"** → scan the session for durable facts. Propose vault entries. Default to vault, not memory.

Extend this list as your team finds patterns worth naming.

---

## When in doubt

- Trust files over recollection. The vault is live; memory is frozen at write time.
- Ask "is the roadmap current?" before suggesting work if anything feels stale.
- Save durable facts to the vault before context clears, not to memory. Ephemeral working state stays in chat.

---

*This file is the agent contract. It changes when the operating loop changes. Keep it tight.*
