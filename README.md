# boredroom.space

Static site for Bored Room. No build step, no JavaScript, no analytics.
Served by GitHub Pages from `main`. The app lives in the `bored-room` repo. This repo is the source of truth for the site: edit it here. `site/` in the app repo is an older snapshot and may carry unreleased copy; don't copy it over this one.

## Fonts and Content-Security-Policy

Instrument Sans is self-hosted in `fonts/` (`@font-face` at the top of `style.css`, licence in `fonts/OFL.txt`); the site makes no third-party requests. Every page has a `Content-Security-Policy` meta tag (`default-src 'self'`, no scripts), so inline `style=` attributes and `<style>` blocks are blocked: add a class in `style.css` instead (one-off tweaks are the `u-` classes at the bottom). New pages need the same meta tag.
