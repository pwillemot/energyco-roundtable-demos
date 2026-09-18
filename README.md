# EnergyCo AI Roundtable — Demo Pages

Self-contained HTML demos for the Energy & Utilities AI Roundtable, styled in the
**Cirrus** demo brand. Designed to run full-screen on a mobile device (via the
Salesforce wrapper app or "Add to Home Screen" in Safari).

## Structure

| Path | What it is |
|------|-----------|
| `index.html` | Landing / **select page** — pick which demo to launch. This is the URL to point the wrapper app at. |
| `crosssell/` | Cross-sell agent: meter reading → planned-interruption notice → EV home-charging cross-sell → site-visit booking. |
| `reschedule/` | Rescheduling agent: a WhatsApp-style conversation to reschedule a technician appointment. |

Each demo is a scripted, self-contained simulation — no backend, no login.

## Publishing (GitHub Pages)

Served from the repository **root** on `main`:

1. Push this folder to a GitHub repo (see setup notes).
2. Repo **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main` / `(root)`.
3. Live at `https://<user>.github.io/<repo>/` — open on the device or point the wrapper app there.

## Running locally

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server
```
