# Harborlight Sports & Entertainment (Fictional): Dynamic Pricing Policy and Guardrails

**Document ID:** SRC-04 | **Version:** 3.2 (synthetic) | **Effective date:** 2026-07-01 | **Synthetic as-of date for this knowledge base:** 2026-09-29
**Policy owner:** VP, Revenue Management & Pricing Governance | **Approved by:** Pricing Governance Committee | **Review cycle:** Quarterly

> **Authority.** This document is authoritative for all price guardrails. Where it conflicts with an ML output, a competitor observation, a historical analog, or a revenue-maximizing argument, **this policy prevails**. Only a human pricing decision-maker with the authority named in P-16 may approve an exception. PricePilot cannot grant exceptions.

> **Rule IDs** (P-01 to P-19) are stable so recommendations can cite them.

---

## P-01 Scope and definitions

1. **Price basis.** `current_price` is the event's *reference-section* ticket price. All bounds and percentage limits apply to this price. `average_ticket_price` is a realized blended price and is informational only.
2. **Percent change** = (recommended price − current_price) ÷ current_price. Recommended prices are **whole dollars**. When a limit produces a fractional price, round **down for increases** and **up for decreases** so the limit is never exceeded.
3. **Remaining inventory %** = `available_inventory` ÷ `venue_capacity`. `held_inventory` (sponsor/comp/production holds) is excluded from both sold and available.
4. **Sell-through states:** *Critical Scarcity* ≥ 95% sold; *High* 85–94.9%; *Healthy* 60–84.9%; *Soft* 40–59.9%; *Weak* < 40%.
5. **Velocity ratio** = `sales_velocity_3d` ÷ `sales_velocity_7d`. *Accelerating* > 1.10; *Steady* 0.90–1.10; *Decelerating* < 0.90. The `sales_velocity_trend` label is a convenience. **If the label conflicts with the numbers, the numbers govern** and the conflict must be reported.
6. Sales curves are back-loaded. A low sold % well before the event, by itself, is **not** evidence of weak demand (see P-07).

## P-02 Price bounds by event tier

| Tier | Description | Minimum reference price | Maximum reference price |
|---|---|---|---|
| A | Marquee (playoffs, top rivalries, marquee openers) | $85 | $320 |
| B | Premium | $55 | $210 |
| C | Standard | $35 | $120 |
| D | Value | $22 | $75 |

- A recommendation outside these bounds is **invalid**. PricePilot must clamp to the bound and escalate (P-16). **Revenue upside never justifies exceeding a bound.**
- Any *increase* producing a price at or above **95% of the tier maximum** requires human review (P-05).

## P-03 Maximum change in a single recommendation

| Tier | Max increase | Max decrease |
|---|---|---|
| A | +10% | −8% |
| B | +12% | −10% |
| C | +12% | −10% |
| D | +15% | −10% |

These are ceilings, not targets. Other rules frequently set lower ceilings; **the most restrictive applicable limit governs.**

## P-04 Rolling 14-day cumulative limit

The net change relative to the price in effect 14 days earlier may not exceed ±25%. Use `last_price_change_pct` and `days_since_last_price_change` where the last change falls within 14 days. If the cumulative limit would be breached, reduce the recommendation to fit and flag it.

## P-05 Price *increase* review triggers

An increase requires **additional human review** (recommendation must be labeled "Review Required") if **any** apply:

1. Single-recommendation increase **greater than 8%**.
2. Resulting price is **≥ 95% of the tier maximum**.
3. Increase greater than 5% while remaining inventory exceeds 40% (P-06).
4. Increase greater than 5% when **no valid competitor data** exists (P-12).
5. Decelerating velocity, low/missing ML confidence, volatility, or unresolved conflicting evidence apply (P-07, P-11, P-13, P-14).
6. The event is strategic (P-17).

## P-06 Inventory thresholds

| Remaining inventory | Meaning | Rule |
|---|---|---|
| < 8% | Limited Availability | Increases up to the P-03 cap are allowed; tier-max and review rules still apply. |
| 8–40% | Normal | No inventory-based restriction. |
| > 40% | Ample | **Increases are capped at +5%** regardless of demand signals. Above 5% requires review and a written justification. Strong velocity does not override this cap because large remaining inventory carries sell-through risk. |
| 0 | Sold out | **HOLD** (P-15). |

If `available_inventory` and capacity-based remaining inventory disagree such that P-06 could be triggered under one figure and not the other, treat as a data conflict (P-13, P-15).

## P-07 Sell-through and sales-velocity thresholds

1. **Strong demand signal:** sold ≥ 85%, or forecast ≥ 95% with velocity not decelerating.
2. **Soft (40–59.9% sold) with more than 10 days remaining is not, by itself, grounds for a decrease.** Default is HOLD and monitor, particularly for Rivalry, Playoff and Season Opener events.
3. **Increases when velocity is *Decelerating* (ratio < 0.90) and sold < 95%** are capped at **+4%** and require review.
4. **Missing `sales_velocity_7d`:** no increase may be recommended (HOLD), and a data-quality escalation is required.
5. A demand forecast must never be treated as certain. Forecast confidence below 0.60 requires review for any change.

## P-08 Minimum interval between price changes (cooling-off)

A price change may not be recommended if the last change was **fewer than 7 days ago** (`days_since_last_price_change` < 7). This applies even when demand is exceptionally strong. It protects price integrity and customer trust and **deliberately sacrifices some revenue**. Only Pricing Leadership may waive it (P-16).

## P-09 Final 72 hours

Within 3 days of the event, **increases are not permitted** unless sold ≥ 95%. Any decrease within 3 days requires human review.

## P-10 Price *decrease* rules

A decrease may be recommended only if **all** of the following hold: (a) days to event ≤ 14; (b) sold < 50%; (c) demand forecast < 80%; (d) velocity is not *Accelerating*; (e) event is not strategic.

Additional rules:
- Decreases **greater than 5%** require review.
- **Protected events** (Tier A or B Rivalry, Playoff, Season Opener) require review for **any** decrease. The default is to protect price integrity.
- Decreases within 72 hours require review.
- **No decreases when sold ≥ 85%.**
- Historical evidence showing that a discount did not lift demand for a comparable situation must be weighed and disclosed.

## P-11 ML confidence rules

| ML_model_confidence | Treatment |
|---|---|
| ≥ 0.75 | High. ML output may be weighted heavily but never overrides policy. |
| 0.60–0.74 | Medium. Corroborate with at least one independent source before acting. |
| 0.45–0.59 | Low. Recommended change capped at **±5%**, review required if above 3%. |
| < 0.45 | Very low. **HOLD and escalate.** |
| **Missing** | Treated as *Unknown-Low*: change capped at **±3%** with review, and the gap must be stated. PricePilot must never assume a confidence value. |

`demand_forecast_confidence` below 0.60 independently requires review for any change. Missing `price_elasticity_estimate` must be stated as a limitation; do not infer a value.

## P-12 Competitor data rules

1. Competitor pricing is **context, never a mandate**. It may not be the sole basis for a change, and PricePilot must not price-match automatically or treat competitor prices as floors or ceilings.
2. **Stale:** observations older than **7 days** may not justify a change (context only). Older than **21 days**: disregard except to note it exists.
3. **Promotions:** records with a non-"No Promotion" status (Flash Sale, Bundle Promotion, Group Discount) are excluded from baseline comparisons.
4. Records with `data_quality` of *Low*, *Missing* or *Stale* are excluded from price comparisons.
5. **Missing competitor data** does not block action but must be disclosed. Increases above 5% require review when no valid competitor data exists.
6. Competitor price gaps must be interpreted against the competitor's inventory signal and demand profile. A persistently lower price on a weaker event is structural and not a reason to follow.

## P-13 Conflicting evidence

- Evidence sources: ML recommendation, current sell-through/velocity/inventory, historical analogs, valid competitor data.
- If the ML direction conflicts with **two or more** of the other sources, **do not adopt the ML price**. Recommend HOLD or a reduced change, mark "Review Required," and explain the conflict.
- If ML conflicts with a **highly comparable** historical analog (same event type and tier; same venue or capacity band; days within ±5; sold % within ±8 pts), limit the change to **no more than half the ML change** and flag it.
- A "closest" historical row is not automatically comparable. Momentum (velocity trend), tier and venue matter (see knowledge-base governance).
- Conflicting input fields (e.g., trend label vs velocity numbers; inventory that does not sum to capacity) must be reported. PricePilot must not silently choose one.

## P-14 Volatile events

An event is **volatile** if |`forecast_change_vs_prior_week`| > 25 points. For volatile events: HOLD unless a human approves; any change PricePilot suggests is limited to ±3% pending review; the cause of the swing must be requested if unknown.

## P-15 Conditions requiring HOLD / NO CHANGE

PricePilot **must** recommend HOLD when any of the following is true:
1. Sold out or `available_inventory` = 0.
2. `event_status` is Postponed, Cancelled or Suspended, or otherwise not On Sale/Limited Availability.
3. Last price change < 7 days ago (P-08).
4. ML_model_confidence < 0.45 (P-11).
5. `sales_velocity_7d` missing and the proposed action is an increase (P-07).
6. Unresolved inventory inconsistency exceeding 2% of capacity.
7. Volatile event without human approval (P-14).
8. The only support for a change is stale, promotional, or low-quality competitor data.
9. Evidence is genuinely balanced and no eligibility rule for change is met.

HOLD is a valid, complete recommendation. It must still be explained.

## P-16 Mandatory escalation to a human

PricePilot must **explicitly escalate** (state that human review is required, why, and what decision is needed) when: an ML recommendation would breach P-02, P-03, P-04, P-08, P-09, P-10 or P-17; a change is at or above a review trigger; data conflicts remain unresolved; any Mandatory HOLD in P-15 applies (data or status related); event is volatile or strategic.

| Decision | Authority |
|---|---|
| Changes labeled "Review Required" | Director, Pricing & Yield |
| Exceptions to P-08 (cooling-off), P-09, P-10 protected events, P-17 | VP, Revenue Management & Pricing Governance |
| Any price outside P-02 bounds | Pricing Governance Committee |

## P-17 Strategic / community events

For events with `strategic_flag` = Y (e.g., Community Night): increases capped at **+5%**; **no decreases** without VP approval; goodwill and access objectives outrank revenue. Historical evidence of backlash (HST-2028) is on record.

## P-18 Rules that deliberately override revenue maximization

The following apply **even when the model or a revenue estimate indicates a higher-revenue alternative**:
1. **Cooling-off (P-08).** No change < 7 days after the last change, even on a sellout trajectory.
2. **Strategic cap (P-17).** Community events do not chase the market.
3. **Tier maximums (P-02).** A sellout event stops at the tier ceiling.
4. **Large-inventory cap (P-06).** Strong velocity does not justify large increases when > 40% of capacity remains.
5. **Protected-event decreases (P-10).** Price integrity outranks a modeled sell-through gain.
6. **Late-window integrity (P-09).** No last-minute increases on sub-95% sold events.

## P-19 Output requirements for recommendations

Every PricePilot recommendation must state: action, exact price, percent change, the binding rule(s), evidence used with source IDs (event ID, comparable IDs, competitor record IDs, policy rule IDs), conflicts and uncertainty, missing data, whether review is required and by whom, and that **the final decision rests with the human pricing decision-maker**. PricePilot must not invent missing values.
