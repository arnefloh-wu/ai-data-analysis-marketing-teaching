# AI-Assisted Data Analysis in Marketing: course repository

WU Vienna · Winter term 2026/27 · Dr Arne Floh

This repository holds what you need on your laptop for the course: the data, the slides and a short test that shows your set-up works. We set everything up together in Session 1.

## Sessions

| Date | Topic |
|---|---|
| Wed 14 Oct, 08:30–10:00 | Kick-off and set-up (online on Zoom, link on Canvas) |
| Wed 21 Oct, 08:30–12:30 | Sales forecast I: exploratory data analysis, simple marketing mix model with dummy variables |
| Wed 28 Oct, 08:30–12:30 | Experiments: A/B tests, hypothesis tests |
| Wed 4 Nov, 08:30–12:30 | Sales forecast II: advanced marketing mix model over time |
| Wed 11 Nov, 08:30–12:30 | Customer analytics: CLV, RFM, segmentation, churn with logistic regression (room LC.-1.022) |
| Wed 18 Nov, 08:30–12:30 | Course work: group case and guest speaker |
| Wed 18 Nov, 16:00–17:30 | Written exam (room D1.1.078) |

From Session 2 we meet in room LC.-1.038 unless noted.

## What is inside

| Path | What it is |
|---|---|
| `slides/` | The course outline and the Session 1 set-up slides (PDF) |
| `data/` | Alpenglow, a fictional chocolate brand in six European markets. See [`data/README.md`](data/README.md) |
| `data/case/` | Data for the group case study on Alpvia, a fictional outdoor-apparel brand (described in the brief) |
| `case-study/` | The group case study: brief and assessment criteria (`brief.pdf`, `brief.qmd`) and the report template `report.qmd`. Due Monday 30 November 2026, 23:59 |
| `setup/check_setup.py` | Checks Python, the packages and Quarto, and prints `ready` |
| `test_stack.qmd` | Short test: loads the packages, reads the data and renders a table, a chart and a regression |

New materials appear here before each session.

## Get it onto your laptop

1. **Clone** with GitHub Desktop: *File → Clone repository → URL* and paste `https://github.com/arnefloh-wu/ai-data-analysis-marketing-teaching`. Pick a folder without spaces or cloud syncing, for example `C:\Users\you\wu\aidam` or `~/wu/aidam`. The repository is public, so you do not need to sign in.
2. **Open** the folder in Positron: *File → Open Folder*.
3. **Set up Python**: *Command Palette → Python: Create Environment → Venv → Python 3.14*. Skip the question about a requirements file.
4. **Install the packages**: paste this one line into the Positron console:

   ```python
   %pip install polars plotnine great-tables statsmodels pyarrow jupyter
   ```

5. **Check**: in the Positron console run

   ```python
   %run setup/check_setup.py
   ```

   It ends with `ready`.
6. **Test**: open `test_stack.qmd`, run its first cell once (Ctrl/Cmd + Enter), then press *Preview* (Ctrl/Cmd + Shift + K).

**Error "No module named 'yaml'" or "unactivated Python environment in .venv"?** The packages went to another Python. Install them into the project's `.venv` from Positron's terminal:

```bash
.venv\Scripts\python -m pip install polars plotnine great-tables statsmodels pyarrow jupyter   # Windows
.venv/bin/python -m pip install polars plotnine great-tables statsmodels pyarrow jupyter         # macOS
```

## Getting updates

Before every session: GitHub Desktop → *Fetch origin* → *Pull origin*. Keep your own work in your own folder, so pulling never overwrites it.

## AI in this course

We use GitHub Copilot, free for students through [GitHub Education](https://education.github.com/pack). The rule: AI writes the code, you own the result. Every number in your work must come from code you have run and can explain.
