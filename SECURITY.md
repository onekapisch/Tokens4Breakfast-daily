# Security & Privacy

Tokens 4 Breakfast is built local-first. This document explains exactly what data is handled and where it goes.

## Data flow
- **Storage:** all usage and settings live in a local SQLite database on your Mac (`~/Library/Application Support/Tokens 4 Breakfast`). Nothing is synced to a server we control.
- **Claude Code:** usage is read from local session files on disk. No API key, no network call to read it.
- **Other providers (OpenAI, Cursor, Gemini, GitHub Copilot, OpenRouter, DeepSeek, Mistral):** queried directly from your Mac using **your own API keys / local credentials**, solely to fetch usage and cost.
- **No telemetry:** the app sends no analytics, no crash pings, and no usage data to us or any third party.
- **No account:** there is no login and no user identifier.
- API keys are stored locally and are never transmitted anywhere except to the corresponding provider's official API.

## Reporting a vulnerability
Please email **kapisch@icloud.com** with details and steps to reproduce. Do not open a public issue for security reports. We aim to respond within 72 hours.
