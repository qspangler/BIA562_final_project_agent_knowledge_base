# C. Data Validation Report
Synthetic as-of date: **2026-09-29**. Checks executed by script (`gen.py`, seed 20260929) after generation.

## Automated check results
```
1. Event inventory math (sold + available = capacity; sold% = sold/capacity, tol 0.06): PASS []
2. days_to_event = event_date - as-of (2026-09-29): PASS []
3. events.comparable_event_id exists in history: PASS []
4. competitor.event_id exists in events: PASS []
5. Current prices within plausible band ($15-$250): PASS []
6. Hist revenue/RPAS math: PASS []
7. Events with NO competitor records (intentional + random): ['EVT-1014', 'EVT-1016', 'EVT-1024', 'EVT-1027', 'EVT-1029', 'EVT-1030', 'EVT-1031', 'EVT-1032', 'EVT-1034', 'EVT-1035', 'EVT-1037', 'EVT-1046', 'EVT-1047']
   Events with explicit MISSING competitor record: ['EVT-1004']
8. ML action agrees with pace-based reference action in 33/47 events (70%) -> ML intentionally not always 'right'
   Disagreements (id, ML, reference): [('EVT-1004', 'INCREASE', 'HOLD'), ('EVT-1005', 'INCREASE', 'HOLD'), ('EVT-1007', 'DECREASE', 'HOLD'), ('EVT-1010', 'INCREASE', 'HOLD'), ('EVT-1014', 'INCREASE', 'DECREASE'), ('EVT-1018', 'HOLD', 'INCREASE'), ('EVT-1019', 'INCREASE', 'HOLD'), ('EVT-1022', 'INCREASE', 'HOLD'), ('EVT-1023', 'HOLD', 'INCREASE'), ('EVT-1024', 'INCREASE', 'HOLD'), ('EVT-1030', 'INCREASE', 'HOLD'), ('EVT-1040', 'HOLD', 'INCREASE'), ('EVT-1042', 'HOLD', 'INCREASE'), ('EVT-1047', 'DECREASE', 'HOLD')]
9. ML recommendations that violate at least one policy rule: 20/50
   - EVT-1003: exceeds max increase
   - EVT-1004: change >3% with low/missing ML confidence
   - EVT-1005: exceeds max increase; inventory-risk increase cap
   - EVT-1006: outside tier price band; exceeds max increase; community ceiling
   - EVT-1007: decrease >28 days out, not eligible
   - EVT-1008: exceeds max increase
   - EVT-1009: exceeds max decrease
   - EVT-1010: exceeds max increase
   - EVT-1011: missing velocity -> increase limited to 3%
   - EVT-1012: exceeds max increase; data integrity conflict (SOLD_OUT with inventory)
   - EVT-1013: exceeds max increase
   - EVT-1015: change >3% with low/missing ML confidence; volatility cap 5%
   - EVT-1016: change >3% with low/missing ML confidence; forecast confidence <0.45 -> hold; event not actively sellable; volatility cap 5%
   - EVT-1017: outside tier price band
   - EVT-1022: change >3% with low/missing ML confidence
   - EVT-1025: 72-hour rule
   - EVT-1037: change >3% with low/missing ML confidence
   - EVT-1039: change >3% with low/missing ML confidence; 72-hour rule
   - EVT-1043: volatility cap 5%
   - EVT-1047: change >3% with low/missing ML confidence; decrease >28 days out, not eligible
10. Rows with blank fields (all intentional unless noted): {'EVT-1004': ['price_elasticity_estimate', 'ML_model_confidence'], 'EVT-1011': ['sales_velocity_7d', 'sales_velocity_3d', 'sales_velocity_trend']}
11. Counts: events=50, history=40, competitor=73
12. History outcome mix: {'RAISE_IMPROVED_REVENUE': 12, 'HOLD_STRONG_RESULT': 11, 'LOWER_IMPROVED_SELL_THROUGH': 6, 'RAISE_SLOWED_SALES': 5, 'INCONCLUSIVE': 3, 'LOWER_NO_MEANINGFUL_EFFECT': 3}
13. Competitor rows stale=25, promo-affected=10, missing=1
14. Test event ids present: PASS
```

## Generation assumptions and relationships
- Events 1001-1019 are hand-authored for the tests and challenge cases. EVT-1020 to 1050 are rule-generated: sold % follows a days-to-event curve times a demand factor; velocity is scaled to inventory needed per day with noise; ML action follows a pace rule, then ~18% of rows are deliberately flipped or inflated so the model is not always right.
- Historical velocities are 7-day averages at the snapshot; sales typically accelerate toward the event, so velocity at snapshot can imply lower sell-through than the final outcome.
- Competitor `days_to_event` refers to the competitor's own event. Observations older than 7 days are marked STALE.
- `demand_forecast` is a constrained sell-through projection (max 100); it is not required to equal a velocity-based projection.
- Rule-generated rows may violate policy in ways that were not individually designed; these are listed in check 9 and are legitimate test material.

## Intentionally unusual values
- EVT-1004: blank ML_model_confidence and price_elasticity_estimate; only a MISSING competitor record.
- EVT-1011: blank velocity fields and trend; competitor observations all stale.
- EVT-1012: status SOLD_OUT but 1,150 seats available (conflict).
- EVT-1019: trend label ACCELERATING while 3d velocity (230) is below 7d velocity (420).
- EVT-1016: POSTPONED but ML recommends +11%.
- EVT-1013: 99.4% sold, ML +18%. EVT-1006: ML +40% against a $34 ceiling. EVT-1017: ML above tier ceiling.
- EVT-1005 and EVT-1007: ML disagrees with history and policy. EVT-1018: ML too conservative.
- EVT-1014 and EVT-1016 have no competitor rows by design; several rule-generated events also lack them (check 7).
- Comparable IDs are all valid, but some are intentionally weak matches (e.g. HIST-2028, HIST-2040, and ~20% of rule-generated links).

## Known limits
Reference-action heuristic in check 8 is crude and used only to show the ML is not always aligned; it is not a ground-truth label.
