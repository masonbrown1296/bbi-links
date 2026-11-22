# bbi-links

Link-in-bio page for Bio Behavioral Institute's Instagram (@bio.behavioral). Static site on GitHub Pages, no build step.

- `index.html`: the page. Design-system colors and type (pine `#0e4144`, mint `#bbf6e7`, Instrument Serif and Sans). Mobile first.
- `links.json`: the links. Two lists:
  - `timed`: shown once `from` has passed and hidden at `until` if set. Newest first, eight at most. Set `from` to the post's publish time (ISO 8601 with the Eastern offset) and the link appears on its own when the post goes live.
  - `pinned`: always shown at the bottom (consultation, referral, articles, phone).
- Links to biobehavioralinstitute.com carry `utm_source=instagram&utm_medium=social&utm_campaign=link_in_bio`. External links carry nothing.

To change the page: edit `links.json`, commit, push. GitHub Pages redeploys in about a minute. The source of truth for what should be on the page and when lives in the cortex repo (`engagements/bbi/content/social/start-page-links.md`); each social batch adds its rows there and here together.

Marketing links only. Nothing in this repo is private.
