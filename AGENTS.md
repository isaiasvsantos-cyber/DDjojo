# Base44 Dev Environment

## Project Overview
This is a single-page static HTML site (`index.html`) served by nginx.

## Setup
- `docker compose -f docker-compose.base44.yml up -d --build` starts nginx on host port 3000.
- The repo root is bind-mounted into nginx's html directory, so edits to `index.html` are reflected immediately on browser refresh.

## Verification
- `curl -s http://localhost:3000/` returns the HTML page.
- No external credentials or services are required.
