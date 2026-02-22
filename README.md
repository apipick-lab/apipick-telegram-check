# apipick-telegram-check

A [Claude Code](https://claude.ai/claude-code) skill that checks whether a phone number is registered on Telegram using the [apipick](https://www.apipick.com) Telegram Checker API.

## What it does

Given a phone number with international country code, this skill returns:

- **Registration status** — whether the number is on Telegram
- **User ID** — Telegram user identifier
- **Username** — public @username if available
- **Name** — first and last name if publicly visible
- **Data center** — Telegram DC ID

Only publicly available Telegram profile information is returned.

## Requirements

An apipick API key is required. Get 100 free credits at [apipick.com](https://www.apipick.com).

## Installation

Install via Claude Code:

```bash
claude skills install https://github.com/apipick-lab/apipick-telegram-check
```

## Usage

Once installed, just ask Claude naturally:

- *"Is +1234567890 registered on Telegram?"*
- *"Check if this number uses Telegram: +8613800138000"*
- *"Find the Telegram username for +447911123456"*

Claude will call the apipick API and report the registration status and any available profile info.

## API Reference

| Field | Value |
|-------|-------|
| Endpoint | `POST https://www.apipick.com/api/check-phone-telegram` |
| Auth | `x-api-key` header |
| Cost | 1 credit per request |

See [`references/api_reference.md`](references/api_reference.md) for full documentation.

## Links

- [apipick.com](https://www.apipick.com) — API platform
- [Telegram Checker](https://www.apipick.com/check-phone-telegram) — product page
- [Get API Key](https://www.apipick.com/dashboard/api-keys)
