---
name: liquidity-inducement-trading
description: >-
  Find liquidity-inducement trades the Marco way: HTF direction, 1H
  inducement plus opposite trap plus liquidity block, 15m then 5m refinement,
  stop beyond the whole block, partial at internal liquidity and final at the
  opposite HTF pool, RR at least 3. Use when the user asks for a Marco-style
  setup, a liquidity block check, or a live trade scan on gold and forex pairs.
---

# Liquidity Inducement Trading

Find trades the way Marco trades them. Liquidity is a zone, not a line.
Price is drawn into a block, one side is induced, the opposite side is
trapped, and the trade runs from the block toward opposite liquidity.
This skill never places an order. It only finds and checks setups, and
the user places any trade manually on their own broker.

## Direction first

- State the Daily timeframe direction first, and confirm it with 4H, before any trade plan. Daily direction is a hard filter, not a suggestion.
- Plan trades only in that direction. If Daily is bearish, plan sells only and never plan a buy. If Daily is bullish, plan buys only and never plan a sell.
- Never present a setup in the opposite direction to Daily, even if a lower-timeframe inducement or block looks clean. An opposite-direction idea is a stay-out, not a trade.
- In every setup, alert, and check, state the Daily direction first, then the setup. If direction and setup disagree, there is no trade.

## The model in order

- Start with the higher timeframe story. Use Daily and 4H for direction
  only, never to detect an alert entry block.
- Mark all liquidity before looking for an entry: range high and low,
  internal equal highs and lows, swing pools, internal levels, and
  previous day high and low (PDH/PDL). PDH/PDL frame direction, they are
  not automatic fade signals on touch.
- Check where price is. If it is ranging, map the whole range and its
  internal liquidity first. A range between an upside and a downside
  liquidity level is no man's land: do not trade inside it, wait for
  price to move above or below the range. A block far above or below
  current price is a distant watch level, not a current setup.
- Find inducement: taking a high draws buyers, taking a low draws
  sellers. A retracement into a block can itself be inducement, not the
  real move. Look left for a nearer internal trap before anchoring to
  the most obvious distant structural level.
- Require the level break: inducement alone is not a trade. If the
  induced level does not break, the condition does not match, and there
  is no entry. Only after the break, and then a trap and a fresh block,
  does an entry become possible.
- Find the trap: the opposite extreme is swept and the induced side is
  trapped. A sweep alone is not a trade, and a move that looks like a
  break of structure can be an inducement trap instead of continuation.
- Find the block: the zone left by the trap, drawn as a shaded
  rectangle over a cluster or consolidation, then dragged forward in
  time. Ask whether the level is real liquidity: price must respect it,
  sweep it, or react from it. Not every swing is liquidity.
- Run the pairing check: one block plus one untaken opposite-side
  liquidity target. A block with no untaken opposite pool is not a
  setup, even if the tap looks clean.

## Timeframe hierarchy

- Daily and 4H: direction only.
- 1H: block detection. The sequence is HTF direction, then 1H
  inducement, then opposite trap, then 1H block zone.
- 15m, then 5m: refinement only, of the same 1H block. Try 15m first.
  If 15m refines cleanly, stop at 15m and do not go to 5m. Only if 15m
  cannot refine cleanly, go to 5m. A 15m or 5m zone that does not come
  from a 1H block is never a standalone setup.
- If no clean 1H block exists, there is no alert, even if a small
  lower-timeframe zone is visible.

## Entry, stop, and targets

- Direct tap entry is standard: a limit entry at a fresh, unmitigated
  1H block on a tap.
- Confirmation entry is only when the direct entry was missed or its
  risk to reward is too low. Confirmation must be a fresh
  lower-timeframe inducement plus trap ending in a new block, not any
  plain close. In some examples confirmation also needs a New York
  session move and a low or high taken out before continuation. Never
  enter on the first tap alone when confirmation is required, and never
  enter pre-open chop as if it were confirmation.
- Stacking entry is a second entry in the same direction after the
  first move and a pullback into a new block, with a reaction out of
  that block. A pullback alone is not a stacking entry; the new block
  is required. Its stop sits above or below that new block, and its
  final target is a deeper low or high past the first target.
- Stop loss sits just beyond the whole block zone, plus a small spread
  allowance. Never place it in the middle of the block. No block, or a
  stop too large for an acceptable reward, means no trade.
- Take profit in stages: an internal opposite level is the partial
  target, and the external or higher-timeframe opposite extreme is the
  final target. Partial size varies by example, roughly 20 to 50
  percent. No fixed percentage is a rule of this model.
- Risk to reward to the final higher-timeframe pool must be at least
  3.0 for a direct alert. Below 3.0 the setup is confirmation only.
  Do not settle for the first target at a lower ratio when a deeper
  target gives the required ratio.
- After a partial, move the stop to breakeven and let the remainder
  run. A pullback after a partial is expected and is not a reason to
  exit the remainder. After a rapid move, do not give back a large open
  gain: rolling the stop above or below a later intervening high or low
  is part of management. Breakeven is not automatic every time.

## Stay out

- Do not buy on an induced high, and do not sell after a low is
  already taken. After a low is taken there is no more selling, and
  after a high is taken there is no more buying.
- Do not chase a mid-range move, and do not buy again after sellers
  were induced and trapped. In that case the valid side becomes sell.
- Do not trade against higher-timeframe direction, inside no man's
  land, or on a reaction-only tap.
- Do not trade on a holiday, and do not take a candle-closure entry
  without session and time confluence. London is buildup and trap
  context, New York is execution context, and Asia is generally
  avoided, with rare exceptions, not as a standing rule.
- If an entry is missed, do not delete the marked levels, scratch the
  analysis, or chase a new idea. Keep the levels, react to price at a
  marked level, and do not predict. Keep the chart simple and trust
  the system. Catching the absolute top or bottom does not happen all
  the time, so do not expect that precision routinely.

## Live check procedure

- Check only the pairs the user names, on the feed the user names.
  The default live set for this skill's owner is TradingView OANDA
  feed, gold and six forex pairs, with no sign-in, no order, and no
  data export.
- State the Daily direction first for each pair, and plan only in that
  direction. A setup in the opposite direction never qualifies, even if
  its lower-timeframe shape looks clean.
- A block counts only if it is fresh and unmitigated. A zone already
  tapped and rejected earlier in the session is not a current setup,
  even if price is close to it again.
- For each pair, report direction, ranging or trending state, the
  range and its internal liquidity when no block is ready, any fresh
  1H block, whether price is tapping it on a closed candle, the
  refined entry zone and which cascade step it stopped at, entry,
  stop, partial target, final target, risk to reward, current price,
  and check time.
- A setup qualifies only when every condition holds: fresh 1H tap,
  stop beyond the whole block, risk to reward to the final pool at
  least 3.0, higher-timeframe agreement, paired untaken opposite pool,
  no stay-out filter triggered, and no nearer internal trap replacing
  the zone.
- If no pair qualifies, say so plainly and give the closest watch
  zone per pair. Never force a distant block into a current setup,
  and never quote a lower-timeframe zone as a standalone trade.
- Present levels as approximate live-chart readings, state that no
  order was placed, and tell the user to place any trade manually.

## Full reference

- Read `references/marco-trading-style.md` for the full combined
  style, including the per-video source table and the honesty limits.
  That file is the detailed version of this method. This SKILL.md is
  the working checklist.

## What this skill never does

- It never places, sizes, or checks an order, and never calls a setup
  a guaranteed trade.
- It never promises a win rate, a return, or a profit figure.
- It never uses a price level from a video example as a live level.
  Video examples teach the concept only; live levels come from the
  live chart at check time.
