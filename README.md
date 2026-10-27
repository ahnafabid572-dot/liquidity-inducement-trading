# Liquidity Inducement Trading

A trading skill built from 16 visually checked Marco / InterEquityTrading
videos: how Marco finds a liquidity block, takes an entry, sets a stop loss
and take profit, and manages the trade.

This is an independent synthesis of publicly shared trading concepts. It is
not an official Marco product, and it is not financial advice. It never
places an order; any trade is placed manually by the user on their own broker.

## What is inside

- `SKILL.md` — the working method and checklist. Load this skill when you
  want a Marco-style setup check or a live scan.
- `references/marco-trading-style.md` — the full combined style, with the
  per-video source table, the stay-out filters, the session rules, and the
  honesty limits (what was seen visually, and what was not).

## The model in one paragraph

Daily and 4H give direction only. On 1H, find inducement, then an opposite
trap, then a liquidity block. Pair that block with an untaken opposite
liquidity pool. Refine the same block on 15m first, and only go to 5m if 15m
cannot refine it. Enter on a tap at the block, stop just beyond the whole
block, take a partial at an internal level, and run the rest to the
higher-timeframe pool, with risk to reward of at least 3 to the final target.
If there is no fresh 1H block, no confirmation, or a stay-out filter is
triggered, there is no trade.

## Pairs and feed used by the owner

TradingView OANDA feed: XAUUSD, EUR/USD, GBP/USD, USD/JPY, USD/CAD, GBP/JPY.
Checks run every 30 minutes, 10:00 to 22:00 Asia/Dhaka, with a silent rule:
no message unless a new qualifying setup forms.

## Install in Muse

Copy this folder to `~/workspace/custom-skills/liquidity-inducement-trading/`
and the skill becomes available through `muse.skill_search`.

## Install in Claude Code

Copy this folder to `~/.claude/skills/liquidity-inducement-trading/` (user
scope) or to `<project>/.claude/skills/liquidity-inducement-trading/`
(project scope), then restart Claude Code or run `/skills` to verify it
appears.
