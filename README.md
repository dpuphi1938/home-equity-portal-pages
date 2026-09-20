# home-equity-portal-pages

Post-close "Home Equity Portal" pages for closed *purchase* transactions,
published by the `transaction-portal` CLI (`ninja-realtor/transaction-portal`).
These replace the active-transaction client portal once a deal closes — no
more timeline/milestones/FAQ, just an ongoing home-value/equity reference and
a way to stay in touch (see `portal/render.py`'s `_is_post_close_purchase`).

**This repo is public (required for free GitHub Pages), but nothing here is
discoverable.** There is deliberately no root `index.html` and no page lists
the transactions that exist — each one lives at `/<slug>/`, where `<slug>` is
a long random token. The URL itself is the access control, the same trust
model already used for MLS share links. Don't add an index/directory page
here; doing so would defeat that.

Source data (client names, addresses, loan terms) lives locally and privately
in `transaction-portal/data/` and is never committed here — only the
rendered HTML output is.
