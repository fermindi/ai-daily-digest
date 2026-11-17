# AI Brief (ai-daily-digest)

Git-backed archive of my Daily AI Brief.

- `PROMPT.md` — the instructions each brief is written from.
- `ROUTINE_PROMPT.md` — the prompt for the daily Claude Code routine (claude.ai → Routines), which runs at 5:47am America/Sao_Paulo with this repo attached.
- `briefs/YYYY-MM-DD.md` — one brief per day.

## How the daily run works

1. Reads the last 5 files in `briefs/` so it can skip repeats, cover only new developments on ongoing stories, and correct earlier errors.
2. Researches the last ~24–26 hours and writes the brief following `PROMPT.md`.
3. Saves it as `briefs/YYYY-MM-DD.md` (São Paulo date), commits to `main`, pushes, and returns the full brief in the chat reply.

To change what the brief covers or how it reads, edit `PROMPT.md` — the next run picks it up.
