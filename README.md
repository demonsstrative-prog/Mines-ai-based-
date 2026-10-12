# Mines AI Signal Bot

A private Telegram bot that helps you play Mines games with AI-based pattern analysis.
**No hacking. No prediction. Only real math + AI analysis of your history.**

Built for personal use. Runs locally. Uses Ollama (free, offline AI) on your laptop.

---

## What it does

1. `/start` → recommends best Mines game for Pakistan with reasoning + link
2. Confirms you're ready → shows rules, risks, money management, disclaimer
3. Asks bomb count → generates a fresh 5x5 safe pattern
4. You play, then tap Loss 🔴 or Win 🟢
5. Bot asks for a screenshot of your result
6. AI reads the screenshot, analyses the round, generates a new safe pattern
7. Repeat — the bot learns your history and adjusts strategy

**What it does NOT do:**
- Predict the next mine location (impossible — server RNG)
- Hack or exploit the game
- Guarantee wins

---

## Requirements

- **Laptop or PC** with:
  - Python 3.10+
  - Ollama installed (https://ollama.com)
  - 8+ GB RAM (16 GB recommended)
- **Telegram account** + bot token from @BotFather

---

## Step 1 — Install Ollama

Download from https://ollama.com and install.

Then pull two models:

```bash
ollama pull llava:7b
ollama pull llama3.2:3b
