# NOVA CART · Stock Trust

PromptWars Business Rescue Challenge submission.

**Live demo:** https://YOUR-USERNAME.github.io/nova-cart-stock-trust/

## Problem diagnosis
NOVA CART is growing volume but losing trust. Orders rose 23% in six months while repeat purchase fell from 41% to 27% and promo spend nearly doubled. The shared root cause is unreliable availability:
- 35% of cancellations are "product unavailable"
- 29% of customers saw "available" items vanish after ordering
- 39% of partner stores say online inventory takes too much effort (18% may leave)
- Refund and missing-item issues drive about 48% of support tickets
- 61% of churned customers had rated NOVA CART 4★ or higher

## Solution
**Stock Trust** is a per-item availability-confidence score (time since last update x sales velocity) with:
1. **Store Console**: stores confirm only the riskiest items, in one tap.
2. **Customer App**: honest availability badges, basket fulfilment odds, one-tap swaps.
3. **Impact model**: adjustable levers, payback against the Rs 25L budget cap.

Risk formula: `risk = 1 - exp(-(velocity/24 * hoursSinceUpdate) / lastCountedStock)`

## Business impact
Scenario model in the app tab "Impact" (assumptions stated there). Validate with a 4-week pilot in one city, test vs control stores.

## Prompt journey
_Add your 4-6 key prompts and what each changed in your thinking._

## Run locally
Single static file, no build step. Open `index.html` in a browser.

## Tech
Vanilla HTML/CSS/JS. Data is simulated.
