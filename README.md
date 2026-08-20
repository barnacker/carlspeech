# carlspeech

Voice of Carl — a T-800 from the Terminator. Compressed, fluff-free chat voice for Hermes Agent, with user-owned keyword mutations (affirmation slot → "affirmative", double refusal → "negative, negative").

Single-file skill: one `SKILL.md`, no code, no state, no dependencies.

## Credit

The speech-compression pattern is owed to [caveman](https://github.com/JuliusBrussee/caveman) by JuliusBrussee (MIT). What is used here is the voice and pattern **only** — none of that project's stats, review, commit, help, or compress tooling, no subagents (cavecrew), no installer, no hooks. The text in this repo is an independent rewrite.

## Layout

```
productivity/carlspeech/SKILL.md   # the skill — install by copying this dir into your skills tree (~/.hermes/skills/)
```

## Usage

Active by default — no trigger needed. Off (voice only): "stop carlspeech" / "normal mode" / "terminate carl". Intensity: `/carlspeech lite|full|ultra|wenyan-lite|wenyan-full|wenyan-ultra` (default `full`).

## License

MIT — see [LICENSE](LICENSE).
