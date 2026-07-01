# Fintrack
AI-powered daily investment digest bot built with n8n, NewsAPI and OpenRouter — covers stocks, mutual funds, crypto, commodities and more, delivered via Telegram
# 📊 Daily Investment Digest Bot (n8n)

An automated n8n workflow that sends a daily Telegram message 
covering Indian stocks, mutual funds, commodities, crypto, 
FD rates and macro economy news — powered by NewsAPI and OpenRouter.

## Features
- 50+ investment topics covered daily
- AI-powered sentiment analysis (Positive/Negative/Neutral/Mixed)
- Grouped by category (Stocks, MF, Crypto, Economy etc.)
- Delivered to Telegram every morning at 8:30 AM

## Stack
- n8n (workflow automation)
- NewsAPI (news headlines)
- OpenRouter / Llama 3.1 (sentiment analysis)
- Telegram Bot API (delivery)

## Setup
1. Import the workflow JSON into your n8n instance
2. Add your NewsAPI key in the Fetch News Headlines node
3. Add your OpenRouter API key as Header Auth credential
4. Create a Telegram bot via @BotFather and add credentials
5. Set your Telegram Chat ID
6. Activate the workflow
