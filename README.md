# Nginx Reverse Proxy Kit

> Visual Nginx config generator: upstreams, TLS, caching, gzip, rate-limit.

**Category:** DevOps  
**Built with:** Nginx, Let's Encrypt, Docker, Bash  
**Author:** Hesam Kazemi — [HessiKz](https://github.com/HessiKz) · Full-Stack & AI Developer

---

## Live demo

This project ships a self-contained interactive demo that runs entirely in the
browser (no backend secrets required), powered by a shared design-system, chart,
and graph engine. It is deployed automatically to **GitHub Pages** on every
push to `main` via the included GitHub Actions workflow.

👉 https://HessiKz.github.io/nginx-reverse-proxy-kit/

## Features

- Interactive, client-side visualisation of the DevOps concept
- Real-time charts, agent/topology graphs, and terminal-style traces
- Responsive dark UI built on a shared component engine
- One-command CI: build + deploy to GitHub Pages

## Tech stack

- **Nginx**
- **Let's Encrypt**
- **Docker**
- **Bash**

## Run locally

```bash
# Clone this repository
git clone https://github.com/HessiKz/nginx-reverse-proxy-kit.git
cd nginx-reverse-proxy-kit

# Serve the static site (any static server)
python3 -m http.server 5173
# or
npx serve .

# Open http://localhost:5173
```

> The browser demo is fully functional standalone. Backend-style projects
> (FastAPI / NestJS / Go) include the conceptual implementation notes in the
> live demo and are structured to drop into a real service.

## Project structure

```
nginx-reverse-proxy-kit/
├── index.html          # App shell (relative paths → works on Pages)
├── styles.css          # Shared design system
├── engine.js           # DOM / chart / graph helpers
├── manifest.js         # Project metadata
├── app.js              # Interactive demo (this project's VIEW)
├── .github/workflows/  # CI → GitHub Pages deploy
└── LICENSE             # MIT · Hesam Kazemi
```

## Credits

Crafted by **Hesam Kazemi** ([@HessiKz](https://github.com/HessiKz)).
Part of a 25-project portfolio demonstrating full-stack, AI, and DevOps
engineering. License: MIT.
