---
marp: true
theme: default
paginate: true
class: lead
---

# Learning with AI

## Sports Betting Analytics & Stock Market Analysis

**Joshua Day**

---

# How I Used AI

- Used AI as a research assistant
- Asked models to explain concepts, math, and terms from scratch
- Kept asking "why" and "what's the catch" until things actually clicked
- Cross-checked answers between models to make sure it was good responses
- No production code, no betting, no trading — just learning

---

# The Models I Used

- Claude (main explainer — concepts and math walkthroughs)
- ChatGPT (second opinion when one explanation didn't land)
- Gemini / Perplexity (quick fact-checks on stats and finance terms)

---

# Topic 1: Sports Betting Analytics

- How sportsbooks set odds and build in their margin
- Expected value, variance, and bankroll management
- Predictive baselines like Elo and Poisson distributions
- What a positive-EV line actually means and why it matters

---

# Core Concepts I Researched

- Implied probability: convert odds to a percentage, then remove the book's cut
- Expected value: how much a bet is worth on average over many attempts
- Kelly criterion: size your bets as a fraction of bankroll to survive the swings
- Closing line value: did your bet beat the final market line? That's the real skill test

---

# Expected Value — What AI Taught Me

- A book listing Team A at 2.10 implies roughly a 47.6% win probability
- If you honestly estimate the real chance at 52%, that's a meaningful edge
- On a $100 bet, that edge works out to about $9.20 of expected profit per wager
- The formula is simple — the hard part is honestly estimating the probability

---

# Kelly Criterion & Variance

- Kelly tells you what fraction of your bankroll to risk given your edge
- Full-Kelly is mathematically optimal but brutally volatile in practice
- Half- or quarter-Kelly trades a little growth for survivable losing streaks
- AI kept making the same point: variance, not the sportsbook, is the real opponent

---

# Predictive Baselines: Elo & Poisson

- Elo rates teams by win/loss history and updates after every game
- Applied to college football, Elo correctly calls roughly 74% of games
- Poisson models how many goals or points a team is likely to score
- A model can be accurate and still not beat the closing line — that's the trap

---

# Topic 2: Stock Market Analysis

- Market mechanics — exchanges, order types, and how market makers work
- Fundamental analysis — reading financial statements, P/E ratios, growth
- Technical analysis — candlesticks, moving averages, momentum indicators
- Risk-adjusted returns and the biases that inflate most backtests

---

# Fundamental vs. Technical

- Fundamental analysis reads the business: earnings, margins, debt, and valuation
- Technical analysis reads the chart: price, volume, and momentum signals
- Fundamental thinking plays out over months to years; technical over days to months
- Biggest takeaway from AI: the strongest signals show up on both at the same time

---

# Moving Averages — Concept Walkthrough

- The 50-day and 200-day simple moving averages smooth out daily noise
- Golden cross: the 50-day crossing above the 200-day is treated as bullish
- Death cross: the reverse, treated as a warning sign
- By themselves these are lagging indicators — useful for context, not for timing

---

# Relative Strength Index (RSI)

- RSI compares recent gains to recent losses over a rolling window (usually 14 days)
- Above 70 is traditionally "overbought"; below 30 is "oversold"
- AI was blunt about it: RSI is a confirmation tool, not a buy or sell signal on its own
- Every shortcut I asked about had a real counter-example the model surfaced immediately

---

# Risk-Adjusted Returns & Backtest Biases

- Sharpe and Sortino ratios measure return relative to the risk taken
- Survivorship bias, look-ahead bias, and transaction costs quietly inflate most backtests
- A strategy that looks great on paper often falls apart once you account for these
- The best-performing backtests are usually the ones that have been tuned too many times

---

# AI Research Tips That Stuck

- Ask why, not just how — definitions are cheap, reasoning is the actual payoff
- Ask for trade-offs and limitations, not just the "right" answer
- Cross-check confident claims against a second model or a real source
- Treat AI confidence as a hypothesis, not a conclusion

---

# Conclusion

- Sports betting and stock analysis share one core skill: quantifying uncertainty honestly
- Evidence before confidence: I never accepted an AI answer until I understood the reasoning
- Without AI I wouldn't have covered this much ground in one semester — but the understanding is mine
