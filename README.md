# dataset-tidy

Fine-tune data hygiene: dedup, length filter, train/valid split

Small but I use it weekly.

## Getting started

```bash
# stdlib only
```

## How to use

```bash
python prep.py raw.jsonl --out-dir data/ --valid-ratio 0.1
```

## What it does

- Deterministic split with a seed
- Length filters keep the sweet spot
- Prints a stats summary you can eyeball
- Dedup by normalized instruction text

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── roadmap.md
│   └── usage.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
└── prep.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
