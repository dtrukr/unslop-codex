# unslop

Empirically detect the repetitive defaults a model falls back on, then turn those findings into a reusable instruction file that makes future outputs less generic.

## Send This To Your Agent

Copy and send this sentence:

```text
Clone https://github.com/dtrukr/unslop-codex, read https://github.com/dtrukr/unslop-codex/blob/main/skills/unslop/SKILL.md, run unslop for DOMAIN_HERE, review unslop-output/analysis.md and unslop-output/skill.md for specificity, and return the finished skill file plus the main repeated patterns you found.
```

Agent-readable instructions live here: [`skills/unslop/SKILL.md`](skills/unslop/SKILL.md)

## What It Does

Every model has defaults it collapses toward. In writing, that means the same openings, transitions, and rhetorical moves. In visual work, that means the same landing-page structure, the same gradients, the same card grids, the same CTA blocks.

`unslop` measures those defaults instead of guessing at them.

1. You give it a domain.
2. It generates a prompt set and produces many samples with Codex.
3. For visual work, it renders screenshots so the analysis can inspect what the pages actually look like.
4. It analyzes the whole set for repeated patterns.
5. It writes `skill.md`, a focused file of what to avoid next time.
6. It runs a before/after comparison so you can see whether the profile actually changed the result.

The main output is a single markdown file you can reuse in Codex, `AGENTS.md`, Cursor rules, or any system prompt.

## Quickstart

You need the Codex CLI installed.

```bash
git clone https://github.com/dtrukr/unslop-codex.git
cd unslop

python3 -m venv .venv
source .venv/bin/activate

# Text / writing domains
python3 unslop.py --domain "blog writing"

# Visual / website domains
pip install playwright && playwright install chromium
python3 unslop.py --domain "startup SaaS landing pages" --type visual --count 20 --concurrency 3
```

## Output

Results land in `./unslop-output/`:

```text
unslop-output/
  skill.md
  analysis.md
  prompts.json
  samples/
  screenshots/
  before-after/
    before.md / before.html
    after.md / after.html
    before.png / after.png
```

`skill.md` is the file you usually want to keep and reuse.

## Common Commands

```bash
python3 unslop.py --domain "marketing emails" --count 50 --concurrency 5
python3 unslop.py --domain "startup SaaS landing pages" --type visual --count 20 --concurrency 3
python3 unslop.py --domain "Python tutorials" --count 100 --concurrency 10
python3 unslop.py --domain "React landing pages" --type visual --model sonnet --effort low
```

## Options

| Flag | Default | Description |
|---|---|---|
| `--domain` | required | What to analyze |
| `--type` | `text` | `text` for writing/code/prose, `visual` for websites/HTML |
| `--count` | `50` | Number of samples to generate |
| `--concurrency` | `5` | Parallel Codex calls |
| `--model` | Codex default | Codex model name to pass through |
| `--effort` | Codex default | Codex reasoning effort to pass through |
| `--timeout` | `600` | Seconds to wait per Codex call |
| `--analysis-timeout` | `1800` | Seconds to wait for the analysis pass |
| `--retries` | `1` | Retries per failed Codex call |
| `--output` | `./unslop-output` | Where to put results |
| `--skip-comparison` | `false` | Skip the before/after step |

## Prebuilt Profiles

The `profiles/` directory contains ready-to-use profiles:

- [`profiles/writing.md`](profiles/writing.md)
- [`profiles/react-design.md`](profiles/react-design.md)

Run the tool yourself when you want something narrower or domain-specific.

## Philosophy

`unslop` focuses on what to avoid, not on prescribing a single new template. The point is to remove the defaults that keep repeating and force the model to make fresher choices.

## Requirements

- Codex CLI
- Python 3.10+
- For visual domains: `pip install playwright && playwright install chromium`

## License

MIT
