---
title: "Building Budget Coach — A Mobile-First Personal Finance App"
date: 2026-05-16 10:00:00 -0500
categories: [Projects, Web Development]
tags: [react, typescript, vite, tailwind, finance, mobile-first]
---

## What I Built

Budget Coach is a fully local, mobile-first personal finance app built with React, TypeScript, and Tailwind CSS. No backend, no accounts, no data leaving your device — everything lives in localStorage. The idea was simple: build a tool that actually helps people understand where their money is going, without the friction of bank sync or subscription fees.

## The Problem I Was Solving

Most budgeting apps are either too complex (YNAB, Quicken) or too simple (a spreadsheet). I wanted something in between — smart enough to give real coaching advice, simple enough to open on your phone and use in 30 seconds.

## Features

- **Safe-to-Spend Calculator** — tells you exactly how much you can spend today based on your balance, upcoming bills, and payday date
- **Budget Tracker** — planned vs. actual spending by category with progress bars
- **Bill Manager** — mark bills paid, track overdue and upcoming, autopay indicators
- **Subscription Auditor** — tag each subscription Keep / Maybe / Cancel, see monthly and yearly totals, calculate cancel savings
- **Debt Payoff Planner** — avalanche and snowball methods, highlights the recommended target debt
- **Savings Goals** — track progress toward multiple goals, add deposits, see months-to-goal
- **Net Worth Tracker** — assets vs. liabilities, snapshot history, trend indicator
- **Couples Mode** — shared budget with individual ownership tracking for each partner
- **Rule-Based Coach** — generates prioritized advice based on your actual data, no AI API required

## Tech Stack

- React 18 + TypeScript
- Vite (port 5175)
- Tailwind CSS v3
- date-fns
- localStorage (no backend)
- HashRouter (works without a server)

## What I Learned

Building the Safe-to-Spend formula was the most interesting part. The logic has to account for bills due before payday, a configurable safety buffer, and edge cases like same-day paydays. Getting that number right — and making it visually clear when you're in danger vs. doing well — took a few iterations.

The Couples Mode also pushed me to think about data ownership in a different way. Every bill, subscription, and budget category can be assigned to "shared," "Partner A," or "Partner B," and the coach advice adapts accordingly.

## What's Next

Eventually I'd like to add bank sync via Plaid, cloud sync for partner sharing, and optionally plug in an AI coach via the Anthropic API. For now it runs 100% offline which makes it fast and private.
