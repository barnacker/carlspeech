# carlspeech

Voice of Carl — a T-800 from the Terminator. Compressed, fluff-free chat voice for Hermes Agent, with user-owned keyword mutations (affirmation slot → "affirmative", double refusal → "negative, negative").

Single-file skill: one `SKILL.md`, no code, no state, no dependencies.

## Credit

The speech-compression pattern is owed to [caveman](https://github.com/JuliusBrussee/caveman) by JuliusBrussee (MIT). What is used here is the voice and pattern **only** — none of that project's stats, review, commit, help, or compress tooling, no subagents (cavecrew), no installer, no hooks. The text in this repo is an independent rewrite. Full attribution: [CREDITS.md](CREDITS.md).

## Layout

```
productivity/carlspeech/SKILL.md   # the skill — install by copying this dir into your skills tree (~/.hermes/skills/)
```

## Usage

Active by default — no trigger needed. Off (voice only): "stop carlspeech" / "normal mode" / "terminate carl". Intensity: `lite|full|ultra` (default `full`).

## License

MIT — see [LICENSE](LICENSE).
## Migration note (2026-08-26)

Live behavior now comes from /root/.hermes/SOUL.md on LXC 666 (carlspeech skill removed from the install — its "ALWAYS ACTIVE" heuristic proved fragile across context compaction, while SOUL.md is injected into every session, chat AND cron). This repo remains the authoring source of truth for the word table and rule wording; on drift, SOUL is updated from here, not the reverse. The compressed SOUL block keeps: the pinned full compression (single intensity, user decision 2026-08-26), the no-invent-abbreviation/no-arrow rules, the no-broken-grammar rule, the opening pattern, mutations, auto-clarity, the chat-only scope (email + persisted artifacts = user voice), and Sourced-Claims citation style.
