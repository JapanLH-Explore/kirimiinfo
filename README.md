# kirimiinfo

The two pages the App Store requires a link to for **ことばの物語 (Kotoba no
Monogatari)**, plus a front page that points at both.

- `support.html` — support page, English and Japanese
- `privacy.html` — privacy policy, English and Japanese
- `index.html` — a front page linking to the two
- `style.css` — shared, and the only stylesheet

Served by GitHub Pages from `main`. Nothing here is built; the files are the
site.

## Why this repo exists separately

The game's source lives in a private repo. These two pages have to be public
because Apple opens them during review, so they live on their own rather than
forcing the game's source, its questions and all four stories' text into the
open.

**Nothing else belongs in here.** In particular, do not publish the built games
(`dist/*.html` from the game repo) to this site. Each one runs standalone in any
browser, and an App Review question about whether an app is a repackaged website
is much harder to answer when the identical game is sitting free on the
developer's own domain.

## Editing

The canonical text is `docs/app-store/privacy-policy.md` and
`docs/app-store/support.md` in the game repo, which explain why each answer is
worded the way it is. Change it there and here together, or the two drift.

Two things that must stay true, because both pages assert them:

- **The app collects nothing.** Adding analytics, crash reporting or anything
  with a server means the privacy page is wrong the day it ships, not later.
- **No third-party requests from these pages.** No fonts, no scripts, no
  analytics, no embeds. A privacy policy that phones somebody on load is its
  own small joke.

## Contact

yukiteachesjapanese@gmail.com
