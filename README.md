# Cebula Skill 🧅

Cebula is an advanced web-scraping and deal-hunting prompt/skill designed for **Agentic Assistants** (such as Claude Code, Cursor, Aider, Cline, and Google Antigravity). It turns your AI assistant into a ruthless bargain hunter specialized in the Polish market.

## Features
- **Price Aggregators**: Automatically scrapes Ceneo and Allegro (prioritizing grouped product listings for the true lowest prices).
- **Amazon Europe**: Systematically checks Amazon PL, DE, FR, IT, and ES, factoring in shipping costs and currency conversions to Poland.
- **Deal Communities**: Scours Pepper.pl, Hotshops.pl, and MyDealz.de for active promotions, expired historical lows, and coupon codes.
- **Second-Hand Market**: Checks OLX and Allegro Lokalnie for used or refurbished options.
- **Anti-Bot Bypass**: Instructs the agent to dynamically switch from standard web fetches to a stealthy headless browser (via Playwright or MCP tools) to bypass enterprise CAPTCHAs like DataDome.

## Prerequisites
To execute this skill successfully, your agent must be equipped with web browsing capabilities (tools like `search_web`, `fetch`, `read_url`, or MCP browser tools).

## Usage & Installation

The core logic is contained inside `SKILL.md`. You can feed this markdown file as context to any capable AI assistant.

### 💻 Claude Code
Claude also supports a skills directory. You can drop `SKILL.md` directly into your Claude skills/prompts configuration folder, or pass the file into your session context dynamically:
```bash
# Example for Claude Code (Context)
claude -p "Read SKILL.md and follow its instructions to find the cheapest Nintendo Switch OLED"
```

### 💻 Aider / Cline
Pass the file directly into your session context, or save it as a custom prompt/architect rule.

### 🪄 Cursor
Copy the contents of `SKILL.md` into your `.cursorrules` file, or add `SKILL.md` to your workspace and `@` mention it in the Composer window to instruct the agent on how to research prices.

### 🚀 Google Antigravity
1. Copy `SKILL.md` to your skills directory: `~/.gemini/config/skills/cebula/SKILL.md`
2. In your chat, simply type: `/cebula [product name]`

## Disclaimer
This skill/prompt is for educational and personal use.
