# Sentinel — Watch-Floor Field Manual

A single-page field manual for **The Sentinel System**: a private, read-only market
watch floor. It explains every function of the stack and how the pieces fit together,
end to end.

- **Warden** — the self-hosted shell that hosts everything.
- **The Recorder** — always-on capture of the live feed into replayable session tapes.
- **The Sentinel Suite** — replays each tape and grades every breakout (the order-flow autopsy).
- **The Research Desk** — mines a month of tapes into one pre-registered, FDR-controlled, sealed-validated framework verdict.
- **The Underwriter** — a read-only 0DTE options screener that never places an order.
- **The Council** — AI persona lenses that read a finished session (and the standalone Board of Directors).

The page carries synthetic (clearly-labeled, invented) readouts and a timestamped
"day on the watch floor" from market open through next-morning review.

## The through-line

The whole system watches, scores, and reports — and **never touches the market**.
Read-only by construction, honest state over fabricated numbers, no look-ahead,
local-only AI reads.

## Run it

It's a single self-contained `index.html` — no build, no dependencies. Open the file,
or serve the folder:

```
python -m http.server 8080   # then open http://localhost:8080
```

## Publish (GitHub Pages)

Settings → Pages → Source: **Deploy from a branch** → Branch: `main` / `/ (root)` → Save.
The site goes live at `https://<user>.github.io/sentinel-field-manual/` within a minute.

---

Every number in the readouts is invented for illustration. The manual documents the
architecture, not live trading data — and there are no credentials or secrets in it.

MIT © Jordan Doerksen
