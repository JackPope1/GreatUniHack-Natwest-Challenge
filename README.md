# Future You: an AI money coach that sees money storms weeks before they hit

**GreatUniHack 2026 · NatWest challenge: AI-Powered Financial Inclusion & Resilience**

▶ **Live demo:** https://jackpope1.github.io/GreatUniHack-Natwest-Challenge/ 

---

## The problem
Jane is a delivery rider and single mum on Universal Credit. Today she has £214 and feels fine. In nine weeks she'll be about £450 short .

She isn't overspending. Her problem is **timing**: rent leaves on the 1st, Universal Credit arrives on the 16th, and a busy December cuts her next UC payment. Banking apps only show what already happened.

## What Future You does
- **The coach speaks first:** it forecasts the next 12 weeks and warns of a "money storm" around 12 January.
- **It explains why**, using Jane's own transactions.
- **It suggests fixes, each tested by simulation**, including support she's entitled to but isn't claiming (UC refunds 85% of childcare costs, about £166 a month). It also writes messages to her landlord or council for her.
- **What-if shocks:** "What if my washing machine breaks next week?"
- **Storm Shield:** a buffer that saves only from spare money and covers dips automatically.
- **12-month view:** from 11 months in the red to none.
- **"Can I afford it?"** checks any purchase against her future, not just today's balance.
- **Accessible:** simple-words mode, large text, high contrast, replies read aloud.

With 8 tested changes, Jane's chance of running short drops from **96% to 2%**.

## How it works
- **Single-page web app**: plain HTML, CSS and JavaScript, with no frameworks and no build step.
- **Forecasting engine (in the browser):** detects bills, income, seasonal and yearly costs, and unclaimed support from 12 months of Open Banking-style transactions. It models the real Universal Credit rules (55% taper, assessment periods, childcare element).
- **Monte Carlo simulation:** 400 possible futures per scenario, from 12 weeks to 12 months, plus shock stress tests. Backtested on October: £91 average error.
- **Claude as the coach:** on claude.ai, typed questions go to Claude, which calls the forecast engine as tools, so it can't invent numbers. Everywhere else, including this repo's live demo, a built-in coach answers the same questions.

## Run it
Open `index.html` in Chrome or Edge, or use the live demo link above. There's nothing to install.

## Responsible by design
It shows how sure it is, explains every prediction, never moves money on its own, is never used for lending decisions, and points to free debt advice (StepChange, Citizens Advice, MoneyHelper) without judgement.

---
*Prototype built at GreatUniHack 2026 by ManHack. All people, companies and figures are synthetic, and the Universal Credit model is simplified.*
