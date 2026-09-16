# tech-challenge-1609

Python 3.14 package managed with uv (`uv_build` backend).

## Commands

- Install: `uv sync --dev`
- Run: `uv run tech-challenge-1609`
- Lint/format (pre-commit: ruff, hygiene, no-comments): `./scripts/check` or `./scripts/check <files>`
- Test: `uv run pytest`

CI (`.github/workflows/ci.yml`) runs `./scripts/check` then `uv run pytest`.

## Layout

- `src/tech_challenge_1609/` — package; `main` in `__init__.py` is the console entry point
- `tests/` — pytest tests
- `scripts/check` — the single definition of "passes"
