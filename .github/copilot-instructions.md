<!-- Copilot instructions for AI coding agents. Keep concise and actionable. -->
# Repo-specific Copilot instructions

Purpose
- This repository is a minimal dataset generator: "random-dataset-generation-10-12-result". The only existing file is `README.md`, which states the project "aims to generate random data set" using 10th vs 12th board results from a particular school.

What an AI agent should know first
- There are no source files, scripts, or tests present. Any changes will introduce code and structure.
- Preserve the single `README.md` and reference it when adding new artifacts.

Primary tasks an agent may perform (prioritized)
- Add a small, self-contained generator (prefer Python or Node depending on user's preference). Place under `scripts/` or `src/` and include a short CLI in `scripts/generate.py` or `scripts/generate.js`.
- Add a small sample output under `data/` (e.g., `data/sample.csv`) demonstrating expected columns and value ranges.
- Add a `README.md` section describing how to run the generator and what the outputs look like.

Project conventions and expectations for edits
- Keep changes minimal and well-scoped: introduce one feature per PR (generator, sample data, or README enhancement).
- Use clear file names: `scripts/generate.py`, `data/sample.csv`, `tests/test_generate.py`.
- When adding code, include a short usage example at the top of `README.md` showing the exact command to run.

Build / run / test notes (discoverable from repository state)
- There are no build or test toolchains detected. When adding a runtime, also add minimal run/test commands in `README.md`.
- Example run command (if Python is chosen):

```
python scripts/generate.py --rows 100 --out data/sample.csv
```

Integration and external dependencies
- No external integrations discovered. If a library is required, prefer lightweight dependencies and add a `requirements.txt` or `package.json`.

When making suggestions or code changes
- If you introduce a language/runtime, add explicit install/run commands in `README.md`.
- Keep changes reversible and small; avoid restructuring the repo without owner approval.
- When unsure about choices (language, file layout, sample schema), add a short proposal in the PR description and solicit the owner's preference.

Examples from this repo
- Source: `README.md` — the project intent is to "generate random data set" for 10th vs 12th board results. Use this as the single source of truth for domain intent.

If you add files, update these spots
- Update `README.md` with run instructions and a brief explanation of the generated fields.
- Add `data/sample.csv` showing representative rows.

Questions for the repository owner
- Do you prefer Python or Node for dataset generation?
- Are there specific columns or formats expected for the 10th vs 12th results?

If feedback is missing or ambiguous, ask before implementing large changes.
