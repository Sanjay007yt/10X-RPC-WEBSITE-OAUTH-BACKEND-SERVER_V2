# 10X RPC — Lightweight 24/7 Backend Server

Dedicated, lightweight Node.js daemon for maintaining 24/7 Discord Gateway WebSocket connections, rich presence activities, and status rotators.

## Features
- Ultra-lightweight: ~60 MB disk usage (well under 1 GiB free-tier container limits like Orihost/Pterodactyl).
- Built-in HTTP health check endpoint on `PORT` / `SERVER_PORT` for panel monitoring.
- Auto-reconnect and token refresh for Discord Gateway connections.

## Setup on Orihost / Pterodactyl
1. Set **Main file** to `index.js`.
2. Create `.env` in the root folder with:
   - `DATABASE_URL`
   - `DATABASE_URL_UNPOOLED`
   - `SESSION_SECRET`
   - `DISCORD_CLIENT_ID`
   - `DISCORD_CLIENT_SECRET`
   - `DISCORD_BOT_TOKEN`
   - `NEXT_PUBLIC_APP_URL`
   - `DISCORD_REDIRECT_URI`
3. Start the server.
