# ProtoPost — Landing Page

[![Live Site](https://img.shields.io/badge/Live%20Site-protopost.onrender.com-3dffa0?style=flat-square)](https://protopost.onrender.com)
[![Hosted on Render](https://img.shields.io/badge/Hosted%20on-Render-46E3B7?style=flat-square&logo=render&logoColor=white)](https://render.com)
[![Static Site](https://img.shields.io/badge/Type-Static%20HTML-lightgrey?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](https://github.com/pgokul695/ProtoPost/blob/main/LICENSE)

The public landing page for **ProtoPost**, hosted at [protopost.onrender.com](https://protopost.onrender.com).

This is a static frontend-only repository. It exists to give the `protopost.onrender.com` URL a safe, public-facing home — without exposing a live, unprotected gateway instance to the internet.

---

## About ProtoPost

**ProtoPost** is a hackathon-ready local email gateway. It lets developers swap email providers, mock sends, and debug emails without touching their app code.

> 📦 **Main project repository:** [github.com/pgokul695/ProtoPost](https://github.com/pgokul695/ProtoPost)

The main repo contains the full FastAPI backend, the dashboard UI, provider integrations (Resend, Mailtrap, Gmail, custom SMTP), and all documentation. This website repo is only the marketing landing page.

---

## Repository Structure

```
protopost-site/
└── index.html    ← the entire site, self-contained
```

That's it. One file. No build step, no dependencies, no package.json.

---

## Tech

- Pure HTML, CSS, and vanilla JavaScript
- [Syne](https://fonts.google.com/specimen/Syne) + [Space Mono](https://fonts.google.com/specimen/Space+Mono) via Google Fonts
- Favicon embedded as a base64 data URI — no external image hosting
- Zero JavaScript frameworks or CSS libraries

---

## Deploying to Render

This site is deployed as a **Render Static Site** — free tier, no sleep, instant global CDN.

### First-time setup

1. Fork or clone this repo to your GitHub account
2. Go to [render.com](https://render.com) → **New → Static Site**
3. Connect this repository
4. Set the following:

| Field | Value |
|---|---|
| **Name** | `protopost` |
| **Branch** | `main` |
| **Publish directory** | `.` |
| **Build command** | *(leave blank)* |

5. Click **Create Static Site**
6. Render assigns the URL `protopost.onrender.com` based on the service name

### Updating the site

Push to `main`. Render redeploys automatically within ~30 seconds.

```bash
git add index.html
git commit -m "update landing page"
git push origin main
```

---

## Why This Repo Exists

The ProtoPost documentation references `protopost.onrender.com` throughout as an example deployment URL. Without this static page at that address, the URL would either:

- Return a 404 (confusing for anyone who clicks it)
- Serve a live, unauthenticated ProtoPost gateway instance accessible to anyone on the internet

This repo solves both problems — the URL resolves to a proper landing page, and no backend service is exposed publicly.

---

## Related

| Link | What it is |
|---|---|
| [github.com/pgokul695/ProtoPost](https://github.com/pgokul695/ProtoPost) | Main project — full source code, docs, and setup guide |
| [ProtoPost Wiki](https://github.com/pgokul695/ProtoPost/wiki) | Full documentation wiki |
| [Hackathon Quickstart](https://github.com/pgokul695/ProtoPost/blob/main/docs/HACKATHON_QUICKSTART.md) | Get email working in 5 minutes |
| [API Reference](https://github.com/pgokul695/ProtoPost/blob/main/docs/API.md) | REST API docs with code examples |

---

## Credits

Built by [Gokul P](https://gokulp.in) and [Devika P Sajith](https://devikapsajith.netlify.app/).
MIT licensed — same as the main project.
