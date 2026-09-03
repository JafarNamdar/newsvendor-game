# Newsvendor Game

Interactive newsvendor exercises for students. Both notebooks run code-free
via [Voila](https://voila.readthedocs.io/) + [Binder](https://mybinder.org).

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

## For students

**Module 1 (play first, in class):**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2Fnewsvendor_module1.ipynb)

**Module 2 (take home after Module 1):**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/JafarNamdar/newsvendor-game/HEAD?urlpath=voila%2Frender%2Fnewsvendor_module2.ipynb)

Each link spins up a private session per student — no code is shown, only
the instructions and interactive widgets. First click can take 1–2 minutes
to build; after that it's usually under a minute.

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
