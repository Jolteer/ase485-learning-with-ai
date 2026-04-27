---
marp: true
theme: default
paginate: true
header: "Learning with AI — Topic 2: Sports Betting Analytics"
footer: "Joshua Day | ASE 485 | Spring 2026"
---

# Sports Betting Analytics

## Probability and Expected Value

**Joshua Day**
ASE 485 — Spring 2026

---

## Why I Chose This Topic

- I follow college football and have a casual interest in sports betting
- I didn't understand the actual math — how odds are calculated, what makes a bet "good" or "bad"
- Combines statistics, probability, and real-world decision-making
- These are quantitative skills that transfer well to data analysis and software engineering

---

## How I Used AI to Learn

- **Claude** as my primary tutor — walked me through probability, EV, and models step by step
- **ChatGPT** for alternative explanations when a concept didn't land the first time
- **Gemini / Perplexity** for quick fact-checks on statistical terms
- I always asked **"what's the catch?"** — AI was good at surfacing the limitations I wouldn't have thought to ask about
- No actual betting — this was purely a learning exercise

---

## How Sportsbooks Work

- Sportsbooks set odds to attract equal action on both sides of a bet
- They build in a **margin (the vig/juice)** so they profit regardless of the outcome
- Example: both sides at -110 means you risk $110 to win $100 — the $10 difference is the book's cut
- The odds don't reflect the "true" probability — they reflect the book's probability **plus their margin**

---

## Implied Probability

- Every set of odds can be converted to an **implied probability**
- American odds of +150 → implied probability = 100 / (150 + 100) = **40%**
- American odds of -200 → implied probability = 200 / (200 + 100) = **66.7%**
- The total implied probability across all outcomes will exceed 100% — that excess is the book's edge
- Understanding this conversion is the foundation for evaluating any bet

---

## Expected Value — The Core Concept

- **Expected value (EV)** = how much a bet is worth on average over many attempts
- Formula: `EV = (Win Probability × Profit) - (Loss Probability × Stake)`
- Example: Team A at 2.10 odds implies ~47.6% chance; if you estimate the real chance at 52%:
  - EV = (0.52 × $110) - (0.48 × $100) = **+$9.20 per $100 bet**
- **Positive EV** means the bet is mathematically worth making over time
- The formula is simple — **honestly estimating the probability is the hard part**

---

## Kelly Criterion — Sizing Your Bets

- Kelly criterion tells you **what fraction of your bankroll to risk** given your estimated edge
- Formula: `f* = (bp - q) / b` where b = odds, p = win probability, q = loss probability
- **Full Kelly** is mathematically optimal but brutally volatile in practice
- **Half-Kelly or quarter-Kelly** trades a little expected growth for survivable losing streaks
- AI kept making the same point: **variance, not the sportsbook, is the real opponent**

---

## Why Bankroll Management Matters

- Even with a genuine edge, short-term results are dominated by **variance**
- A 55% win rate still produces losing streaks of 8+ games regularly
- Without proper bankroll management, a single bad run can wipe you out before the edge plays out
- This directly parallels budgeting in personal finance — **discipline matters more than any single decision**

---

## Predictive Models: Elo Ratings

- **Elo** rates teams by win/loss history and updates after every game
- Originally designed for chess — adapted to sports by adjusting for margin of victory and home advantage
- Applied to college football, Elo correctly calls roughly **74% of games**
- Simple to implement and understand, but limited by the data it uses
- A model can be accurate and **still not beat the closing line** — that's the trap

---

## Predictive Models: Poisson Distribution

- **Poisson distribution** models how many goals or points a team is likely to score
- Works well for low-scoring sports (soccer, hockey) where scoring events are rare and independent
- Less useful for high-scoring sports like basketball where scoring is more continuous
- AI helped me understand that **model selection depends on the sport's scoring characteristics**

---

## Closing Line Value — The Real Skill Test

- The **closing line** is the final odds before a game starts — it's the most efficient price
- If you consistently bet at better odds than the closing line, you likely have an edge
- If you don't beat the closing line, your wins are probably just **luck masquerading as skill**
- This is the metric professional bettors actually care about — not short-term win rate

---

## My Interpretation — What Actually Stuck

- Sports betting is fundamentally a **math problem**, not a prediction problem
- The house edge means most bettors lose long-term — understanding EV lets you see exactly why
- Responsible bankroll management (Kelly Criterion) is just as important as finding good bets
- **Quantifying uncertainty honestly** is the core skill — the same skill used in investing, ML, and engineering
- Knowing when you _don't_ have an edge is more valuable than finding one

---

## How AI Changed My Understanding

- Before: I thought good betting was about "knowing sports" and picking winners
- After: I understand it's about **finding mispriced odds and managing variance**
- AI was excellent at explaining the math with concrete examples I could follow
- It also surfaced the limitations — like how most "winning systems" fall apart at the closing line
- I verified everything by working through the formulas myself, not just reading explanations

---

## Connection to My Capstone Project

- SmartSpend helps users budget and manage money with ML-powered insights
- Sports betting analytics reinforced the same theme: **math beats intuition**
- Bankroll management maps directly to budget management — both are about surviving variance
- Both domains punish people who ignore the numbers and reward those who track honestly

---

# Questions?

**Repository:** github.com/Jolteer/ase485-learning-with-ai
