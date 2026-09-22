# Cebula Skill 🧅

Cebula is an advanced web-scraping and deal-hunting skill designed for the **Antigravity / Gemini Agent** platform. It specializes in finding the absolute lowest prices on the Polish market.

## Features
- **Price Aggregators**: Automatically scrapes Ceneo and Allegro (prioritizing grouped product listings for the true lowest prices).
- **Amazon Europe**: Systematically checks Amazon PL, DE, FR, IT, and ES, factoring in shipping costs and currency conversions to Poland.
- **Deal Communities**: Scours Pepper.pl, Hotshops.pl, and MyDealz.de for active promotions, expired historical lows, and coupon codes.
- **Second-Hand Market**: Checks OLX and Allegro Lokalnie for used or refurbished options.
- **Anti-Bot Bypass**: Instructs the agent to dynamically switch from standard web fetches to a stealthy headless browser (DevTools MCP) to bypass enterprise CAPTCHAs like DataDome.

## Installation
1. Copy the `SKILL.md` file to your Antigravity skills directory: `~/.gemini/config/skills/cebula/SKILL.md`
2. In your Antigravity chat, simply ask the agent to run the Cebula skill on a product, e.g.:
   > "Użyj skilla cebula żeby znaleźć najtańszą ofertę na Nintendo Switch OLED"

## Disclaimer
This skill is for educational and personal use. 
