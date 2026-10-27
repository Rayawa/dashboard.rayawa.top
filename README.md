# dashboard.rayawa.top

English | [简体中文](README_zh.md)

A multilingual landing site for Dashboard clients, market-data services and API resources.

## Overview

The static site links to Dashboard interfaces and platform clients, describes the service architecture and displays service statistics. It is a presentation layer; the market backend is maintained separately. Team identities and personal contact details are excluded from the landing pages.

## Technology and Dependencies

HTML, CSS and JavaScript, with external fonts/icons and API-supplied statistics. A static HTTP server is sufficient for the page; live counters and configured links depend on the external service.

## Repository Structure

- `index.html` — default landing page
- `en/` — English landing page
- `fr/` — French landing page
- `dashboard.css` — shared presentation styles
- `dashboard.js` — service configuration and statistics

## Quick Start

Run a static server from the repository root:

```bash
python3 -m http.server 8000
```

Open `http://localhost:8000/`. No frontend compilation is required. Network access is needed for externally hosted resources.

Review service URLs in `dashboard.js` before deployment. Use `/en/` or `/fr/` for the other language pages.
