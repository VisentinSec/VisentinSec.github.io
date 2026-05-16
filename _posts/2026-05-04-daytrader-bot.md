---
title: "DayTrader Bot — CHoCH + FVG Automated Trading Strategy"
date: 2026-05-04 10:00:00 -0500
categories: [Projects, Finance, Python]
tags: [python, alpaca, algorithmic-trading, paper-trading, choch, fvg, automation]
---

## What I Built

DayTrader is a standalone automated day trading bot implementing the Craig Percoco Change of Character (CHoCH) + Fair Value Gap (FVG) strategy. It connects to Alpaca Paper Trading by default — no real money at risk. The bot watches for specific market structure setups and executes simulated trades automatically.

## The Strategy

**Change of Character (CHoCH)** is a market structure concept — when price breaks a recent swing high (in a downtrend) or swing low (in an uptrend), it signals a potential trend reversal. Combined with a **Fair Value Gap** (an imbalance in price created by a three-candle move), this strategy looks for entries where price has shown structural intent AND left an inefficiency it's likely to return to fill.

The logic:
1. Identify the current market structure (higher highs / lower lows)
2. Watch for a CHoCH — a break of structure that suggests reversal
3. Wait for price to create a FVG on the move
4. Enter when price returns to fill the FVG, with the CHoCH as confirmation

## Tech Stack

- Python 3
- Alpaca paper trading SDK (alpaca-py)
- yfinance for historical data
- pandas + numpy for signal detection
- Runs as a standalone script, no web UI

## Why Alpaca Paper First

The bot defaults to paper trading because the strategy needs to be validated before any real capital is at risk. I'm tracking win rate, average risk/reward, and drawdown across different market conditions before considering a live account. The goal is consistent performance data, not a single lucky run.

## What I Learned

Implementing the CHoCH detection algorithmically was harder than it sounds. In manual trading, a human eye identifies swing points intuitively. Turning that into a rule-based algorithm — defining exactly what counts as a "significant" swing high or low, how many candles constitute a valid structure break — required a lot of parameter tuning and backtesting.

The FVG detection was more straightforward: three consecutive candles where the wick of candle 1 and the wick of candle 3 don't overlap, with candle 2 being the impulsive move. The gap between them is the FVG zone.

Getting the entry timing right (waiting for price to return to the FVG rather than chasing the initial move) is where most of the edge comes from — and also where patience matters most.
