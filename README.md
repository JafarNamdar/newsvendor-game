# Newsvendor Game — Module 2

Interactive newsvendor case studies for students. Runs code-free for students
via [Voila](https://voila.readthedocs.io/) + [Binder](https://mybinder.org).

## For students

Click the badge below (once you've replaced `YOUR-USERNAME/YOUR-REPO` after
pushing to GitHub — see setup steps):

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/YOUR-USERNAME/YOUR-REPO/main?urlpath=voila/render/newsvendor_module2.ipynb)

The first click can take 1–2 minutes to build. After that it should launch in
under a minute. Students will see only the markdown instructions and the
interactive widgets — no code.

## Setup (one-time, for the instructor)

1. Push this folder to a new **public** GitHub repo (Binder requires public
   repos on the free tier).
2. Go to https://mybinder.org
3. Paste your repo URL, leave the branch as `main` (or whatever your default
   branch is).
4. In the "URL to open" field, choose **URL** (not "File") and enter:
   `voila/render/newsvendor_module2.ipynb`
5. Click **Launch** — this triggers the first build (5–15 min). Grab the
   generated link and/or badge markdown it gives you; that's what you share
   with students going forward.
6. Test the link yourself end-to-end before sending it out.

## Notes

- Binder's free tier is for light, occasional use — fine for a class of
  students working through this over a few days, not for hundreds of
  simultaneous heavy users.
- If the link goes idle for a while, the next person to click it will
  trigger a fresh (slower) build. This is normal and not something you need
  to fix.
- If you'd rather students see (and can edit) the code, drop the
  `voila/render/` prefix from the URL and just link the notebook path
  directly — that opens the normal Jupyter interface instead.
