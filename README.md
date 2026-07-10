# 📊 Fintrack — Daily Investment Digest Bot

AI-powered daily investment digest bot built with **n8n**, **NewsAPI**, and **OpenRouter** — covering Indian stocks, mutual funds, crypto, commodities, FD rates, and macro economy news, delivered straight to Telegram every morning.

---

## ✨ Features

- 🗞️ **50+ investment topics** covered daily across Indian stocks, indices, mutual funds, commodities, and crypto.
- 🤖 **AI-powered sentiment analysis** — each headline tagged Positive / Negative / Neutral / Mixed.
- 🗂️ **Grouped by category** — Stocks, Mutual Funds, Crypto, Economy, FD Rates, and more.
- ⏰ **Delivered every morning at 8:30 AM** straight to Telegram, weekdays only.
- ⚙️ **Fully automated** — no manual triggering, runs end-to-end as an n8n workflow.

---

## 🛠️ Stack

| Component | Technology |
| :--- | :--- |
| ⚙️ **Workflow automation** | n8n |
| 📰 **News source** | NewsAPI |
| 🧠 **Sentiment analysis** | OpenRouter (`meta-llama/llama-3.1-8b-instruct`) |
| 📬 **Delivery** | Telegram Bot API |

---

## 🚀 Setup

1. 📥 **Import** the workflow JSON into your n8n instance.
2. 🔑 **Add your NewsAPI key** in the *Fetch News Headlines* node.
3. 🔐 **Add your OpenRouter API key** as a Header Auth credential.
4. 🤖 **Create a Telegram bot** via [@BotFather](https://t.me/BotFather) and add its credentials to the *Telegram* node.
5. 💬 **Set your Telegram Chat ID** where the digest should be delivered.
6. ▶️ **Activate the workflow** — Fintrack will now run automatically every weekday morning.

---

## 🔄 How It Works

1. ⏱️ A scheduled trigger fires every weekday at 8:30 AM.
2. 📰 The workflow fetches fresh headlines for 50+ topics via NewsAPI.
3. 🧠 Each headline is passed through OpenRouter/Llama 3.1 for sentiment tagging.
4. 🗂️ Headlines are grouped by category (Stocks, MF, Crypto, Commodities, Economy, FD Rates).
5. 📬 A formatted digest is sent to Telegram, respecting Telegram's message character limits.

---

## 📝 Notes

Built as a hands-on exercise in n8n workflow orchestration — chaining scheduled triggers, external API calls, LLM-based sentiment analysis, and message formatting into a single automated daily digest.
