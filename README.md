# Newsvendor Game

Interactive newsvendor exercises for students. Both notebooks run code-free
via [Voila](https://voila.readthedocs.io/) + [Binder](https://mybinder.org).

## 🎮 Play the game

**Module 1 — play first, in class:**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2Fnewsvendor_module1.ipynb)

**Module 2 — take home after Module 1:**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2Fnewsvendor_module2.ipynb)

Click a badge above (or use the direct links below it, if badges don't
render on your device):

- Module 1: https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2Fnewsvendor_module1.ipynb
- Module 2: https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2Fnewsvendor_module2.ipynb

**First click can take 1–2 minutes to build** (it's setting up a private
Python environment just for you) — that's normal, just wait for it. After
that it usually loads in under a minute.

### How to play

1. Read the scenario description at the top of the page.
2. Click **Start / Reset** to begin.
3. Enter your **order quantity** and click **Submit**. You'll see the
   demand that occurred, your profit for that round, and your updated
   running average.
4. Repeat until the round counter says you're done.
5. Click **Download CSV** to save your results — you'll need this file for
   your write-up/submission.
6. Scroll down and answer the questions in that section before moving to
   the next one.

No code is shown anywhere on the page — if you ever see raw Python instead
of a scenario description and buttons, refresh the page or re-click the
link above.

## Course flow

1. **Module 1 (in-class / first play)** — `newsvendor_module1.ipynb`
   Simple discrete-demand intro (5-point distribution, Scenario A/B/Custom).
   Gets students comfortable with the mechanics: order, observe demand, see
   profit, watch the running mean/SD build up.

2. **Module 2 (take-home)** — `newsvendor_module2.ipynb`
   **One product, nine short scenarios**, each isolating exactly one lever
   behind the newsvendor formula: a Co shock, a Cu shock, a proportional
   shock where the ratio (and Q*) stay invariant even though both costs
   change, a demand-mean shock, a demand-uncertainty shock, a service-level
   scenario (no cost given at all), continuous sensitivity curves, and a
   behavioral framing test — plus a final "whole story" chart. Each
   scenario ends with a specific, numbered set of questions to answer (not
   open-ended discussion prompts), so students' write-ups are directly
   comparable across the class. It's a menu,
   not a checklist: the notebook tells students to pick 4 scenarios (always
   including the baseline and the framing chapter) for their 8-minute,
   4-slide presentation — see the guide inside the notebook.

## Setup (one-time, for the instructor)

Already done for this repo — both notebooks and `requirements.txt` are at
the repo root. If you ever add a new notebook, the pattern for its Binder
link is:

```
https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2FYOUR_NOTEBOOK_NAME.ipynb
```

To generate/verify a link yourself on mybinder.org:
1. **GitHub repository name or URL:** `JafarNamdar/newsvendor-game`
2. **Git ref:** `HEAD`
3. **File to open:** change the dropdown from **File** to **URL**, then enter
   `voila/render/YOUR_NOTEBOOK_NAME.ipynb`
4. Click **Launch**, and use the auto-generated shareable URL (not the
   session-specific one in your browser's address bar once it loads).

## Notes

- Binder's free tier is for light, occasional use — fine for a class working
  through this over a few days, not for hundreds of simultaneous users.
- If a link goes idle for a while, the next click triggers a fresh (slower)
  build. Normal, not something to fix.
- If you'd rather students see (and can edit) the code, drop the
  `voila/render/` prefix and just link the notebook path directly — that
  opens the normal Jupyter interface instead.
