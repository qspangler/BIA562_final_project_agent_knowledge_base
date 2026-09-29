# PricePilot Synthetic Data

This file contains synthetic data for testing PricePilot, an AI-augmented college football ticket pricing recommendation system. The data is fictional/synthetic and is intended for testing and demonstration.

## 1. Event Pricing Inputs and ML Outputs

| event_id | event_name | event_type | event_tier | event_date | days_to_event | venue | venue_capacity | tickets_sold | available_inventory | sold_percentage | sales_velocity_7d | sales_velocity_3d | sales_velocity_trend | current_price | average_ticket_price | days_since_last_price_change | demand_forecast | demand_forecast_confidence | price_elasticity_estimate | ML_recommended_price | ML_recommended_action | ML_model_confidence | forecast_change_vs_prior_week | comparable_event_id | strategic_priority | event_status |
|---|---|---|---|---|---:|---|---:|---:|---:|---:|---:|---:|---|---:|---:|---:|---:|---:|---:|---:|---|---:|---:|---|---|---|
| EVT-1001 | Harborline Herons vs Pinecrest Foxes (Oct 13) | Regular Season Game | T2 | 2026-10-13 | 14 | Calder Basin Arena | 18000 | 12960 | 5040 | 72.0 | 310 | 360 | ACCELERATING | 80 | 75 | 9 | 94 | 0.86 | -0.6 | 84 | INCREASE | 0.84 | 2.5 | HIST-2006 | N | ON_SALE |
| EVT-1002 | Harborline Herons vs Ashgrove Lynx (Oct 20) | Regular Season Game | T2 | 2026-10-20 | 21 | Calder Basin Arena | 18000 | 9900 | 8100 | 55.0 | 330 | 320 | STABLE | 76 | 73 | 2 | 90 | 0.79 | -1.2 | 77 | HOLD | 0.76 | -1.0 | HIST-2007 | N | ON_SALE |
| EVT-1003 | Harborline Herons vs Larkspur Wolves (Oct 16) | Regular Season Game | T2 | 2026-10-16 | 17 | Calder Basin Arena | 18000 | 13680 | 4320 | 76.0 | 300 | 250 | DECELERATING | 80 | 76 | 7 | 97 | 0.8 | -0.9 | 89 | INCREASE | 0.78 | 1.5 | HIST-2010 | N | ON_SALE |
| EVT-1004 | Harborline Herons vs Marrow Bay Otters (Oct 11) | Regular Season Game | T2 | 2026-10-11 | 12 | Calder Basin Arena | 18000 | 11340 | 6660 | 63.0 | 520 | 540 | STABLE | 74 | 71 | 8 | 92 | 0.7 |  | 78 | INCREASE |  | 1.0 | HIST-2039 | N | ON_SALE |
| EVT-1005 | Harborline Herons vs Ironwood Bison (Oct 08) | Regular Season Game | T2 | 2026-10-08 | 9 | Calder Basin Arena | 18000 | 12240 | 5760 | 68.0 | 560 | 470 | DECELERATING | 74 | 71 | 6 | 91 | 0.74 | -1.3 | 84 | INCREASE | 0.81 | 0.5 | HIST-2014 | N | ON_SALE |
| EVT-1006 | Community Appreciation Night (Oct 05) | Community Night | C | 2026-10-05 | 6 | Lumen Park Pavilion | 12500 | 11750 | 750 | 94.0 | 210 | 240 | ACCELERATING | 30 | 29 | 10 | 100 | 0.9 | -0.3 | 42 | INCREASE | 0.88 | 1.0 | HIST-2038 | Y | LIMITED_INVENTORY |
| EVT-1007 | Harborline Herons vs Tidewater Kestrels (Nov 02) | Regular Season Game | T2 | 2026-11-02 | 34 | Calder Basin Arena | 18000 | 7380 | 10620 | 41.0 | 170 | 140 | DECELERATING | 72 | 69 | 11 | 84 | 0.62 | -1.0 | 65 | DECREASE | 0.71 | -9.0 | HIST-2013 | N | ON_SALE |
| EVT-1008 | Harborline Herons vs Stonebridge Rams - Rivalry Night (Oct 07) | Rivalry Game | T1 | 2026-10-07 | 8 | Calder Basin Arena | 18000 | 16560 | 1440 | 92.0 | 330 | 380 | ACCELERATING | 132 | 128 | 8 | 100 | 0.88 | -0.5 | 146 | INCREASE | 0.85 | 3.0 | HIST-2025 | Y | LIMITED_INVENTORY |
| EVT-1009 | Harborline Herons vs Copperfield Stags (Oct 03) | Regular Season Game | T3 | 2026-10-03 | 4 | Calder Basin Arena | 18000 | 6840 | 11160 | 38.0 | 150 | 90 | DECELERATING | 42 | 40 | 7 | 46 | 0.8 | -1.4 | 34 | DECREASE | 0.79 | -3.0 | HIST-2019 | N | ON_SALE |
| EVT-1010 | Velvet Orbit Live (Oct 29) | Concert | S | 2026-10-29 | 30 | Ostrander Dome | 22000 | 10560 | 11440 | 48.0 | 400 | 430 | STABLE | 105 | 100 | 10 | 99 | 0.83 | -0.7 | 121 | INCREASE | 0.8 | 4.0 | HIST-2029 | N | ON_SALE |
| EVT-1011 | Harborline Herons vs Tidewater Kestrels - Season Series (Oct 14) | Regular Season Game | T1 | 2026-10-14 | 15 | Calder Basin Arena | 18000 | 11880 | 6120 | 66.0 |  |  |  | 118 | 112 | 12 | 95 | 0.75 | -0.6 | 124 | INCREASE | 0.72 | 2.0 | HIST-2001 | N | ON_SALE |
| EVT-1012 | Herons Exhibition vs Ridgeway Rovers (Oct 08) | Exhibition Game | T3 | 2026-10-08 | 9 | Lumen Park Pavilion | 12500 | 11350 | 1150 | 90.8 | 260 | 250 | STABLE | 38 | 36 | 5 | 100 | 0.85 | -0.4 | 43 | INCREASE | 0.8 | 2.0 | HIST-2021 | N | SOLD_OUT |
| EVT-1013 | Harborline Herons vs Ironwood Bison - Rivalry Finale (Oct 02) | Rivalry Game | T1 | 2026-10-02 | 3 | Calder Basin Arena | 18000 | 17892 | 108 | 99.4 | 60 | 40 | DECELERATING | 150 | 141 | 5 | 100 | 0.93 | -0.3 | 177 | INCREASE | 0.9 | 1.0 | HIST-2027 | Y | LIMITED_INVENTORY |
| EVT-1014 | Frostwing Family Spectacular (Oct 18) | Family Show | T3 | 2026-10-18 | 19 | Fenwick Hall | 6000 | 3120 | 2880 | 52.0 | 95 | 100 | STABLE | 39 | 37 | 9 | 86 | 0.77 | -0.8 | 41 | INCREASE | 0.74 | 1.5 | HIST-2035 | N | ON_SALE |
| EVT-1015 | Harborline Herons vs Ashgrove Lynx - Star Player Questionable (Oct 12) | Regular Season Game | T1 | 2026-10-12 | 13 | Calder Basin Arena | 18000 | 12780 | 5220 | 71.0 | 200 | 120 | DECELERATING | 118 | 113 | 9 | 84 | 0.55 | -0.9 | 112 | DECREASE | 0.52 | -12.0 | HIST-2040 | N | ON_SALE |
| EVT-1016 | Herons Exhibition vs Redfern Falcons (Oct 18) | Exhibition Game | T3 | 2026-10-18 | 19 | Lumen Park Pavilion | 12500 | 5750 | 6750 | 46.0 | 40 | 25 | DECELERATING | 36 | 35 | 14 | 60 | 0.3 | -0.5 | 40 | INCREASE | 0.55 | -20.0 | HIST-2022 | N | POSTPONED |
| EVT-1017 | Harbor Fireworks Night vs Cedar Vale Comets (Oct 10) | Regular Season Game | T3 | 2026-10-10 | 11 | Calder Basin Arena | 18000 | 15120 | 2880 | 84.0 | 380 | 400 | STABLE | 57 | 52 | 6 | 100 | 0.88 | -0.5 | 63 | INCREASE | 0.83 | 3.0 | HIST-2020 | N | ON_SALE |
| EVT-1018 | Harborline Herons vs Redfern Falcons (Oct 06) | Regular Season Game | T2 | 2026-10-06 | 7 | Calder Basin Arena | 18000 | 16200 | 1800 | 90.0 | 400 | 470 | ACCELERATING | 80 | 77 | 8 | 100 | 0.85 | -0.5 | 80 | HOLD | 0.82 | 1.0 | HIST-2015 | N | LIMITED_INVENTORY |
| EVT-1019 | Harborline Herons vs Copperfield Stags - Kids Day (Oct 15) | Regular Season Game | T3 | 2026-10-15 | 16 | Calder Basin Arena | 18000 | 10440 | 7560 | 58.0 | 420 | 230 | ACCELERATING | 44 | 42 | 7 | 90 | 0.74 | -0.9 | 47 | INCREASE | 0.77 | 1.0 | HIST-2020 | N | ON_SALE |
| EVT-1020 | Harborline Herons vs Ironwood Bison (Nov 18) | Regular Season Game | T2 | 2026-11-18 | 50 | Calder Basin Arena | 18000 | 3654 | 14346 | 20.3 | 270 | 302 | STABLE | 76 | 70.33 | 30 | 91 | 0.72 | -1.1 | 75 | HOLD | 0.8 | -1.8 | HIST-2008 | N | ON_SALE |
| EVT-1021 | Herons Exhibition vs Summit Hollow Bears (Nov 23) | Exhibition Game | T3 | 2026-11-23 | 55 | Lumen Park Pavilion | 12500 | 1325 | 11175 | 10.6 | 211 | 271 | ACCELERATING | 37 | 36.03 | 30 | 100 | 0.59 | -0.9 | 37 | HOLD | 0.42 | 13.0 | HIST-2022 | N | ON_SALE |
| EVT-1022 | Glass Harbor Choir Live (Nov 02) | Concert | S | 2026-11-02 | 34 | Ostrander Dome | 22000 | 8734 | 13266 | 39.7 | 220 | 182 | DECELERATING | 99 | 95.54 | 6 | 71 | 0.55 | -1.5 | 105 | INCREASE | 0.44 | 5.0 | HIST-2032 | N | ON_SALE |
| EVT-1023 | Harborline Herons vs Ironwood Bison - Rivalry Night (Oct 08) | Rivalry Game | T1 | 2026-10-08 | 9 | Calder Basin Arena | 18000 | 17730 | 270 | 98.5 | 28 | 22 | DECELERATING | 131 | 130.34 | 12 | 100 | 0.89 | -0.9 | 131 | HOLD | 0.75 | -0.1 | HIST-2027 | N | LIMITED_INVENTORY |
| EVT-1024 | Harborline Herons vs Ironwood Bison (Nov 23) | Regular Season Game | T2 | 2026-11-23 | 55 | Calder Basin Arena | 18000 | 2052 | 15948 | 11.4 | 393 | 490 | ACCELERATING | 71 | 65.48 | 6 | 98 | 0.64 | -1.4 | 74 | INCREASE | 0.66 | 3.0 | HIST-2009 | N | ON_SALE |
| EVT-1025 | Herons Exhibition vs Stonebridge Rams (Oct 03) | Exhibition Game | T3 | 2026-10-03 | 4 | Lumen Park Pavilion | 12500 | 7412 | 5088 | 59.3 | 888 | 962 | STABLE | 37 | 34.92 | 2 | 92 | 0.66 | -1.2 | 36 | DECREASE | 0.52 | 1.3 | HIST-2021 | N | ON_SALE |
| EVT-1026 | Herons Exhibition vs Pinecrest Foxes (Oct 31) | Exhibition Game | T3 | 2026-10-31 | 32 | Lumen Park Pavilion | 12500 | 4375 | 8125 | 35.0 | 171 | 132 | DECELERATING | 38 | 36.43 | 12 | 77 | 0.57 | -0.4 | 38 | HOLD | 0.62 | -1.8 | HIST-2022 | N | ON_SALE |
| EVT-1027 | Harborline Herons vs Redfern Falcons (Nov 22) | Regular Season Game | T2 | 2026-11-22 | 54 | Calder Basin Arena | 18000 | 2322 | 15678 | 12.9 | 348 | 345 | STABLE | 79 | 78.24 | 15 | 100 | 0.92 | -1.4 | 78 | HOLD | 0.95 | 4.2 | HIST-2009 | N | ON_SALE |
| EVT-1028 | Harborline Herons vs Stonebridge Rams (Nov 22) | Regular Season Game | T2 | 2026-11-22 | 54 | Calder Basin Arena | 18000 | 3276 | 14724 | 18.2 | 334 | 459 | ACCELERATING | 74 | 72.38 | 21 | 96 | 0.62 | -1.2 | 75 | HOLD | 0.69 | -2.8 | HIST-2012 | N | ON_SALE |
| EVT-1029 | Harborline Herons vs Ironwood Bison - Rivalry Night (Nov 22) | Rivalry Game | T1 | 2026-11-22 | 54 | Calder Basin Arena | 18000 | 4104 | 13896 | 22.8 | 208 | 262 | ACCELERATING | 131 | 130.03 | 4 | 81 | 0.6 | -1.1 | 132 | HOLD | 0.44 | -13.2 | HIST-2026 | N | ON_SALE |
| EVT-1030 | Teachers & Nurses Night (Nov 24) | Community Night | C | 2026-11-24 | 56 | Lumen Park Pavilion | 12500 | 1212 | 11288 | 9.7 | 268 | 317 | ACCELERATING | 27 | 26.8 | 21 | 100 | 0.83 | -1.0 | 28 | INCREASE | 0.75 | 2.2 | HIST-2037 | Y | ON_SALE |
| EVT-1031 | Harborline Herons vs Pinecrest Foxes (Nov 04) | Regular Season Game | T2 | 2026-11-04 | 36 | Calder Basin Arena | 18000 | 5328 | 12672 | 29.6 | 202 | 275 | ACCELERATING | 80 | 74.97 | 6 | 71 | 0.87 | -1.1 | 80 | HOLD | 0.91 | -13.3 | HIST-2017 | N | ON_SALE |
| EVT-1032 | Herons Exhibition vs Ridgeway Rovers (Oct 11) | Exhibition Game | T3 | 2026-10-11 | 12 | Lumen Park Pavilion | 12500 | 12312 | 188 | 98.5 | 22 | 24 | STABLE | 38 | 34.97 | 21 | 100 | 0.81 | -0.4 | 41 | INCREASE | 0.79 | -4.1 | HIST-2021 | N | LIMITED_INVENTORY |
| EVT-1033 | Teachers & Nurses Night (Nov 01) | Community Night | C | 2026-11-01 | 33 | Lumen Park Pavilion | 12500 | 5262 | 7238 | 42.1 | 143 | 193 | ACCELERATING | 27 | 25.82 | 21 | 83 | 0.51 | -1.1 | 27 | HOLD | 0.44 | -1.2 | HIST-2038 | Y | ON_SALE |
| EVT-1034 | Teachers & Nurses Night (Nov 26) | Community Night | C | 2026-11-26 | 58 | Lumen Park Pavilion | 12500 | 2125 | 10375 | 17.0 | 102 | 83 | DECELERATING | 29 | 28.33 | 9 | 67 | 0.73 | -0.7 | 29 | HOLD | 0.71 | 0.7 | HIST-2036 | Y | ON_SALE |
| EVT-1035 | Hollow Mercury Live (Oct 04) | Concert | S | 2026-10-04 | 5 | Ostrander Dome | 22000 | 17424 | 4576 | 79.2 | 541 | 662 | ACCELERATING | 97 | 93.03 | 21 | 90 | 0.69 | -1.3 | 91 | DECREASE | 0.6 | 5.2 | HIST-2032 | N | ON_SALE |
| EVT-1036 | Harborline Herons vs Ridgeway Rovers (Oct 10) | Regular Season Game | T2 | 2026-10-10 | 11 | Calder Basin Arena | 18000 | 17730 | 270 | 98.5 | 17 | 17 | STABLE | 73 | 70.73 | 15 | 100 | 0.69 | -1.0 | 70 | DECREASE | 0.69 | -2.2 | HIST-2011 | N | LIMITED_INVENTORY |
| EVT-1037 | Saffron Static Live (Oct 21) | Concert | S | 2026-10-21 | 22 | Ostrander Dome | 22000 | 21318 | 682 | 96.9 | 20 | 18 | STABLE | 111 | 107.32 | 6 | 96 | 0.59 | -0.3 | 105 | DECREASE | 0.52 | -6.3 | HIST-2030 | N | LIMITED_INVENTORY |
| EVT-1038 | Glass Harbor Choir Live (Nov 26) | Concert | S | 2026-11-26 | 58 | Ostrander Dome | 22000 | 2640 | 19360 | 12.0 | 274 | 210 | DECELERATING | 110 | 107.84 | 15 | 88 | 0.9 | -1.0 | 109 | HOLD | 0.95 | 0.9 | HIST-2029 | N | ON_SALE |
| EVT-1039 | Harborline Herons vs Redfern Falcons (Oct 03) | Regular Season Game | T2 | 2026-10-03 | 4 | Calder Basin Arena | 18000 | 14976 | 3024 | 83.2 | 1035 | 900 | DECELERATING | 80 | 74.13 | 2 | 100 | 0.59 | -1.0 | 87 | INCREASE | 0.54 | -3.8 | HIST-2015 | N | ON_SALE |
| EVT-1040 | Harborline Herons vs Ridgeway Rovers (Oct 06) | Regular Season Game | T3 | 2026-10-06 | 7 | Calder Basin Arena | 18000 | 16542 | 1458 | 91.9 | 186 | 149 | DECELERATING | 43 | 41.44 | 30 | 98 | 0.59 | -0.5 | 43 | HOLD | 0.6 | 0.8 | HIST-2039 | N | LIMITED_INVENTORY |
| EVT-1041 | Harborline Herons vs Larkspur Wolves (Nov 27) | Regular Season Game | T2 | 2026-11-27 | 59 | Calder Basin Arena | 18000 | 1638 | 16362 | 9.1 | 172 | 172 | STABLE | 80 | 78.79 | 30 | 63 | 0.58 | -0.5 | 80 | HOLD | 0.47 | -5.3 | HIST-2016 | N | ON_SALE |
| EVT-1042 | Harborline Herons vs Cedar Vale Comets (Oct 11) | Regular Season Game | T3 | 2026-10-11 | 12 | Calder Basin Arena | 18000 | 12996 | 5004 | 72.2 | 466 | 530 | ACCELERATING | 46 | 44.55 | 4 | 100 | 0.8 | -1.3 | 46 | HOLD | 0.71 | 2.3 | HIST-2011 | N | ON_SALE |
| EVT-1043 | Harborline Herons vs Summit Hollow Bears (Oct 30) | Regular Season Game | T2 | 2026-10-30 | 31 | Calder Basin Arena | 18000 | 10944 | 7056 | 60.8 | 291 | 287 | STABLE | 82 | 77.59 | 9 | 95 | 0.72 | -0.4 | 88 | INCREASE | 0.72 | -13.1 | HIST-2014 | N | ON_SALE |
| EVT-1044 | Herons Exhibition vs Summit Hollow Bears (Oct 28) | Exhibition Game | T3 | 2026-10-28 | 29 | Lumen Park Pavilion | 12500 | 7875 | 4625 | 63.0 | 141 | 181 | ACCELERATING | 35 | 33.74 | 4 | 96 | 0.68 | -1.3 | 35 | HOLD | 0.66 | 0.1 | HIST-2021 | N | ON_SALE |
| EVT-1045 | Herons Exhibition vs Pinecrest Foxes (Oct 23) | Exhibition Game | T3 | 2026-10-23 | 24 | Lumen Park Pavilion | 12500 | 8225 | 4275 | 65.8 | 167 | 148 | STABLE | 34 | 31.94 | 2 | 100 | 0.69 | -1.5 | 34 | HOLD | 0.57 | -10.3 | HIST-2022 | N | ON_SALE |
| EVT-1046 | Harborline Herons vs Larkspur Wolves (Nov 23) | Regular Season Game | T2 | 2026-11-23 | 55 | Calder Basin Arena | 18000 | 2970 | 15030 | 16.5 | 288 | 373 | ACCELERATING | 78 | 75.5 | 6 | 100 | 0.59 | -0.7 | 78 | HOLD | 0.54 | 6.2 | HIST-2009 | N | ON_SALE |
| EVT-1047 | Harborline Herons vs Larkspur Wolves (Nov 18) | Regular Season Game | T3 | 2026-11-18 | 50 | Calder Basin Arena | 18000 | 5076 | 12924 | 28.2 | 367 | 473 | ACCELERATING | 44 | 43.19 | 9 | 99 | 0.51 | -0.7 | 42 | DECREASE | 0.53 | -6.2 | HIST-2019 | N | ON_SALE |
| EVT-1048 | Harborline Herons vs Redfern Falcons (Nov 12) | Regular Season Game | T3 | 2026-11-12 | 44 | Calder Basin Arena | 18000 | 4572 | 13428 | 25.4 | 243 | 186 | DECELERATING | 47 | 43.49 | 15 | 86 | 0.86 | -1.1 | 47 | HOLD | 0.81 | -2.2 | HIST-2019 | N | ON_SALE |
| EVT-1049 | Teachers & Nurses Night (Nov 22) | Community Night | C | 2026-11-22 | 54 | Lumen Park Pavilion | 12500 | 1650 | 10850 | 13.2 | 120 | 151 | ACCELERATING | 30 | 28.76 | 2 | 66 | 0.6 | -1.5 | 30 | HOLD | 0.64 | -2.0 | HIST-2037 | Y | ON_SALE |
| EVT-1050 | Harborline Herons vs Summit Hollow Bears (Oct 04) | Regular Season Game | T2 | 2026-10-04 | 5 | Calder Basin Arena | 18000 | 12402 | 5598 | 68.9 | 932 | 1021 | STABLE | 80 | 77.61 | 6 | 92 | 0.6 | -1.3 | 80 | HOLD | 0.48 | 1.6 | HIST-2011 | N | ON_SALE |

Major fields are represented directly by their column names. `event_id` identifies the event record. `comparable_event_id` identifies the related historical comparable-event record. `ML_recommended_price`, `ML_recommended_action`, and `ML_model_confidence` contain model output fields. The venue, inventory, sales, price, demand forecast, event tier, event status, and strategic-priority fields describe event-level inputs.

## 2. Historical Comparable Events

| comparable_event_id | event_type | event_tier | season | venue_capacity | days_to_event_at_snapshot | tickets_sold_at_snapshot | sold_percentage_at_snapshot | sales_velocity | average_price | final_average_price | final_sell_through | revenue_per_available_seat | total_ticket_revenue | price_change_action | price_change_pct | price_change_amount | outcome | similarity_notes |
|---|---|---|---|---:|---:|---:|---:|---:|---:|---:|---:|---:|---:|---|---:|---:|---|---|
| HIST-2001 | Regular Season Game | T1 | 2024-25 | 18000 | 14 | 13320 | 74.0 | 320 | 121 | 126 | 98.5 | 124.11 | 2233980 | RAISE | 6 | 7.26 | RAISE_IMPROVED_REVENUE | Similar velocity acceleration; marquee opponent; Friday night. Strong analog for T1 games at ~14 days. |
| HIST-2002 | Regular Season Game | T1 | 2024-25 | 18000 | 15 | 12600 | 70.0 | 290 | 118 | 121 | 96.0 | 116.16 | 2090880 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Held through the window; demand built late without intervention. |
| HIST-2003 | Regular Season Game | T1 | 2023-24 | 18000 | 10 | 9360 | 52.0 | 190 | 116 | 108 | 88.0 | 95.04 | 1710720 | LOWER | -8 | -9.28 | LOWER_IMPROVED_SELL_THROUGH | Weak midweek game; decrease lifted sell-through modestly. Low-demand profile. |
| HIST-2004 | Regular Season Game | T1 | 2023-24 | 18000 | 12 | 11880 | 66.0 | 240 | 125 | 132 | 90.0 | 118.8 | 2138400 | RAISE | 14 | 17.5 | RAISE_SLOWED_SALES | Increase above 10% coincided with ~35% drop in 7d velocity; finished short of forecast (97%). |
| HIST-2005 | Regular Season Game | T1 | 2024-25 | 18000 | 30 | 8100 | 45.0 | 210 | 119 | 122 | 97.0 | 118.34 | 2130120 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Early-window hold; curve was back-loaded, most sales in final 3 weeks. |
| HIST-2006 | Regular Season Game | T2 | 2024-25 | 18000 | 14 | 12780 | 71.0 | 305 | 75 | 80 | 97.5 | 78.0 | 1404000 | RAISE | 7 | 5.25 | RAISE_IMPROVED_REVENUE | Near-identical profile to current mid-tier weekend games: same velocity band, same tier, same venue. |
| HIST-2007 | Regular Season Game | T2 | 2024-25 | 18000 | 21 | 9720 | 54.0 | 260 | 72 | 74 | 88.0 | 65.12 | 1172160 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | On-pace at 3 weeks; hold produced steady build and healthy final average price. |
| HIST-2008 | Regular Season Game | T2 | 2023-24 | 18000 | 20 | 10260 | 57.0 | 265 | 74 | 75 | 89.0 | 66.75 | 1201500 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Elastic demand segment; hold outperformed neighboring game that discounted. |
| HIST-2009 | Regular Season Game | T2 | 2023-24 | 18000 | 18 | 8640 | 48.0 | 160 | 73 | 76 | 84.0 | 63.84 | 1149120 | RAISE | 5 | 3.65 | INCONCLUSIVE | Severe storm two days after change distorted sales; effect of raise cannot be isolated. |
| HIST-2010 | Regular Season Game | T2 | 2024-25 | 18000 | 17 | 14220 | 79.0 | 330 | 79 | 86 | 99.0 | 85.14 | 1532520 | RAISE | 8 | 6.32 | RAISE_IMPROVED_REVENUE | Strong velocity and high sold %; 8% raise absorbed with no slowdown. |
| HIST-2011 | Regular Season Game | T2 | 2023-24 | 18000 | 17 | 13860 | 77.0 | 290 | 78 | 83 | 91.0 | 75.53 | 1359540 | RAISE | 15 | 11.7 | RAISE_SLOWED_SALES | Very similar to HIST-2010 at snapshot, but 15% raise slowed sales and left ~1,600 unsold. |
| HIST-2012 | Regular Season Game | T2 | 2023-24 | 18000 | 33 | 7560 | 42.0 | 170 | 70 | 68 | 87.0 | 59.16 | 1064880 | LOWER | -8 | -5.6 | LOWER_NO_MEANINGFUL_EFFECT | Early discount did not change the (back-loaded) curve; sold same late-window volume, lower price. |
| HIST-2013 | Regular Season Game | T2 | 2024-25 | 18000 | 35 | 7200 | 40.0 | 160 | 71 | 74 | 91.0 | 67.34 | 1212120 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Holiday-adjacent game; 40% sold at 5 weeks was normal for this curve; hold was correct. |
| HIST-2014 | Regular Season Game | T2 | 2023-24 | 18000 | 9 | 11160 | 62.0 | 230 | 74 | 77 | 89.0 | 68.53 | 1233540 | RAISE | 12 | 8.88 | RAISE_SLOWED_SALES | Raise with >35% inventory unsold inside 10 days slowed sales; final sell-through 89% vs 93% forecast. |
| HIST-2015 | Regular Season Game | T2 | 2024-25 | 18000 | 8 | 11880 | 66.0 | 300 | 76 | 77 | 95.0 | 73.15 | 1316700 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Held at 8 days; strong finish without intervention. |
| HIST-2016 | Regular Season Game | T2 | 2023-24 | 18000 | 11 | 10800 | 60.0 | 210 | 76 | 71 | 90.0 | 63.9 | 1150200 | LOWER | -6 | -4.56 | LOWER_IMPROVED_SELL_THROUGH | Weeknight game with soft demand; 6% decrease improved sell-through. |
| HIST-2017 | Regular Season Game | T3 | 2023-24 | 18000 | 12 | 7200 | 40.0 | 150 | 42 | 37 | 70.0 | 25.9 | 466200 | LOWER | -10 | -4.2 | LOWER_NO_MEANINGFUL_EFFECT | Weak opponent draw; 10% decrease did not lift demand meaningfully. |
| HIST-2018 | Regular Season Game | T3 | 2024-25 | 18000 | 14 | 8280 | 46.0 | 190 | 43 | 40 | 84.0 | 33.6 | 604800 | LOWER | -8 | -3.44 | LOWER_IMPROVED_SELL_THROUGH | Value game; discount plus promotion improved sell-through. |
| HIST-2019 | Regular Season Game | T3 | 2024-25 | 18000 | 5 | 7020 | 39.0 | 110 | 42 | 38 | 61.0 | 23.18 | 417240 | LOWER | -10 | -4.2 | LOWER_NO_MEANINGFUL_EFFECT | Late discount inside 5 days did not move volume; low awareness late in window. |
| HIST-2020 | Regular Season Game | T3 | 2024-25 | 18000 | 20 | 9360 | 52.0 | 240 | 44 | 46 | 94.0 | 43.24 | 778320 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | On-pace value game; hold captured full demand. |
| HIST-2021 | Exhibition Game | T3 | 2023-24 | 12500 | 10 | 6250 | 50.0 | 140 | 35 | 33 | 82.0 | 27.06 | 338250 | LOWER | -7 | -2.45 | LOWER_IMPROVED_SELL_THROUGH | Exhibition with modest draw; 7% decrease helped sell-through. |
| HIST-2022 | Exhibition Game | T3 | 2024-25 | 12500 | 7 | 5500 | 44.0 | 90 | 36 | 36 | 68.0 | 24.48 | 306000 | HOLD | 0 | 0.0 | INCONCLUSIVE | Weak interest; unclear whether an earlier change would have helped. |
| HIST-2023 | Exhibition Game | T3 | 2024-25 | 12500 | 16 | 7250 | 58.0 | 190 | 35 | 37 | 90.0 | 33.3 | 416250 | RAISE | 6 | 2.1 | RAISE_IMPROVED_REVENUE | Small raise absorbed; sell-through above forecast. |
| HIST-2024 | Rivalry Game | T1 | 2024-25 | 18000 | 12 | 14760 | 82.0 | 350 | 128 | 138 | 99.5 | 137.31 | 2471580 | RAISE | 8 | 10.24 | RAISE_IMPROVED_REVENUE | Rivalry night with scarce inventory; raise improved revenue with no slowdown. |
| HIST-2025 | Rivalry Game | T1 | 2024-25 | 18000 | 10 | 15840 | 88.0 | 360 | 132 | 143 | 99.2 | 141.86 | 2553408 | RAISE | 10 | 13.2 | RAISE_IMPROVED_REVENUE | Closest analog for high-sell-through rivalry games: sold % 88, velocity high, 10% raise absorbed. |
| HIST-2026 | Rivalry Game | T1 | 2023-24 | 18000 | 11 | 15120 | 84.0 | 330 | 130 | 134 | 94.0 | 125.96 | 2267280 | RAISE | 16 | 20.8 | RAISE_SLOWED_SALES | Raise of 16% overshot; sales slowed sharply and 1,000+ seats went unsold. |
| HIST-2027 | Rivalry Game | T1 | 2023-24 | 18000 | 8 | 16380 | 91.0 | 300 | 135 | 138 | 99.6 | 137.45 | 2474064 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Held at 91% sold; sold out anyway. Small remaining inventory. |
| HIST-2028 | Rivalry Game | T1 | 2024-25 | 18000 | 18 | 14040 | 78.0 | 300 | 125 | 133 | 98.0 | 130.34 | 2346120 | RAISE | 9 | 11.25 | RAISE_IMPROVED_REVENUE | Superficial match: T1 and similar sold % but weaker opponent draw and midweek date; raise worked partly because of a promotion. |
| HIST-2029 | Concert | S | 2024-25 | 22000 | 30 | 11000 | 50.0 | 400 | 104 | 112 | 99.0 | 110.88 | 2439360 | RAISE | 10 | 10.4 | RAISE_IMPROVED_REVENUE | Headline act, strong early velocity; 10% raise absorbed. |
| HIST-2030 | Concert | S | 2023-24 | 22000 | 28 | 10120 | 46.0 | 320 | 106 | 110 | 91.0 | 100.1 | 2202200 | RAISE | 14 | 14.84 | RAISE_SLOWED_SALES | Raise above 10% slowed sales; artist demand less deep than presale suggested. |
| HIST-2031 | Concert | S | 2024-25 | 22000 | 25 | 12760 | 58.0 | 380 | 100 | 104 | 97.0 | 100.88 | 2219360 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Hold produced strong late sales and stable pricing. |
| HIST-2032 | Concert | S | 2023-24 | 22000 | 14 | 11440 | 52.0 | 300 | 98 | 92 | 90.0 | 82.8 | 1821600 | LOWER | -10 | -9.8 | LOWER_IMPROVED_SELL_THROUGH | Underperforming concert; decrease lifted sell-through but revenue per seat fell. |
| HIST-2033 | Family Show | T3 | 2024-25 | 6000 | 15 | 3300 | 55.0 | 90 | 37 | 38 | 93.0 | 35.34 | 212040 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Family show; steady weekend build. |
| HIST-2034 | Family Show | T3 | 2023-24 | 6000 | 12 | 2880 | 48.0 | 70 | 38 | 36 | 80.0 | 28.8 | 172800 | LOWER | -8 | -3.04 | LOWER_IMPROVED_SELL_THROUGH | Soft weekday matinee; discount helped. |
| HIST-2035 | Family Show | T3 | 2024-25 | 6000 | 20 | 3600 | 60.0 | 110 | 38 | 40 | 98.0 | 39.2 | 235200 | RAISE | 5 | 1.9 | RAISE_IMPROVED_REVENUE | Small raise on high-demand holiday show absorbed. |
| HIST-2036 | Community Night | C | 2024-25 | 12500 | 7 | 11625 | 93.0 | 210 | 29 | 29 | 100.0 | 29.0 | 362500 | HOLD | 0 | 0.0 | HOLD_STRONG_RESULT | Community night at ceiling policy; held at community price; sold out with strong goodwill. |
| HIST-2037 | Community Night | C | 2023-24 | 12500 | 9 | 10625 | 85.0 | 200 | 28 | 30 | 99.6 | 29.88 | 373500 | RAISE | 10 | 2.8 | RAISE_IMPROVED_REVENUE | Small raise within ceiling; sold out. |
| HIST-2038 | Community Night | C | 2024-25 | 12500 | 6 | 11250 | 90.0 | 180 | 30 | 33 | 99.0 | 32.67 | 408375 | RAISE | 10 | 3.0 | RAISE_IMPROVED_REVENUE | Raise brought price to just under the ceiling; revenue up but fan-relations complaints elevated (see policy 4.6). |
| HIST-2039 | Regular Season Game | T2 | 2024-25 | 18000 | 16 | 11340 | 63.0 | 250 | 75 | 78 | 95.0 | 74.1 | 1333800 | RAISE | 4 | 3.0 | RAISE_IMPROVED_REVENUE | Modest raise on a mid-tier game with solid velocity; no slowdown. |
| HIST-2040 | Regular Season Game | T1 | 2024-25 | 18000 | 20 | 10440 | 58.0 | 260 | 120 | 116 | 92.0 | 106.72 | 1920960 | LOWER | -5 | -6.0 | INCONCLUSIVE | Competing city event same night confounded results. |

## 3. Competitor / Secondary Market Pricing

| competitor_event_id | event_id | competitor_name | comparable_event_type | ticket_section_or_tier | competitor_price | observation_date | days_to_event | inventory_signal | promotion_status | price_change_vs_previous_observation | data_quality | notes |
|---|---|---|---|---|---:|---|---:|---|---|---:|---|---|
| COMP-3001 | EVT-1001 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 86 | 2026-09-27 | 15 | MODERATE | NONE | 4.9 | HIGH | Raised twice in 10 days; reportedly selling well. Supports ML increase. |
| COMP-3002 | EVT-1001 | GateLine Resale Marketplace | Regular Season Game | Lower Bowl Mid | 91 | 2026-09-28 | 14 | LIMITED | NONE | 3.0 | MEDIUM | Resale median above face value; consistent with strong demand. |
| COMP-3003 | EVT-1002 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 77 | 2026-09-26 | 22 | MODERATE | NONE | 0.0 | HIGH | Flat for three weeks; consistent with hold. |
| COMP-3004 | EVT-1002 | Larkspur Wolves (home game) | Regular Season Game | Lower Bowl Mid | 75 | 2026-09-25 | 21 | MODERATE | NONE | -1.3 | MEDIUM | Minor dip; within normal noise. |
| COMP-3005 | EVT-1003 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 88 | 2026-09-27 | 18 | LIMITED | NONE | 6.0 | HIGH | Raised after strong weekend; supports increase. |
| COMP-3006 | EVT-1003 | Larkspur Wolves (home game) | Regular Season Game | Lower Bowl Mid | 74 | 2026-09-26 | 17 | MODERATE | NONE | -6.3 | MEDIUM | Lowered after a slow weekend; contradicts increase but competitor game has weaker draw. |
| COMP-3007 | EVT-1003 | Ridgeway Live | Regular Season Game | Lower Bowl Mid | 69 | 2026-09-27 | 17 | ABUNDANT | ACTIVE_PROMO | -12.0 | LOW | Fan Fest bundle promo with 2 days remaining; low comparability. |
| COMP-3008 | EVT-1004 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid |  |  |  | UNKNOWN | UNKNOWN |  | MISSING | No comparable competitor event found for this date; scraper returned no records. Do not infer. |
| COMP-3009 | EVT-1005 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 84 | 2026-09-27 | 10 | LIMITED | NONE | 5.0 | MEDIUM | Competitor raising; but their event has a star draw. Moderate comparability. Supports ML on its face. |
| COMP-3010 | EVT-1005 | GateLine Resale Marketplace | Regular Season Game | Upper Bowl | 80 | 2026-09-28 | 9 | MODERATE | NONE | 2.0 | MEDIUM | Resale median modestly above face. |
| COMP-3011 | EVT-1006 | Ridgeway Live | Community Night | General Admission | 55 | 2026-09-26 | 7 | LIMITED | NONE | 0.0 | MEDIUM | Commercial family night; different pricing model, not comparable to a subsidized community event. |
| COMP-3012 | EVT-1006 | Larkspur Wolves (home game) | Community Night | General Admission | 28 | 2026-09-27 | 8 | MODERATE | NONE | 0.0 | HIGH | Community-night comparable; priced at community level. |
| COMP-3013 | EVT-1007 | Larkspur Wolves (home game) | Regular Season Game | Lower Bowl Mid | 59 | 2026-09-28 | 35 | ABUNDANT | ACTIVE_PROMO | -18.1 | HIGH | Flash sale ends in 3 days; temporary; misleading as a price benchmark. |
| COMP-3014 | EVT-1007 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 70 | 2026-09-17 | 36 | MODERATE | NONE | -2.8 | STALE | Observation older than 7 days. |
| COMP-3015 | EVT-1007 | GateLine Resale Marketplace | Regular Season Game | Lower Bowl Mid | 71 | 2026-09-26 | 34 | ABUNDANT | NONE | -1.4 | MEDIUM | Essentially flat vs. our price; no strong signal. |
| COMP-3016 | EVT-1008 | Cedar Vale Comets (home game) | Rivalry Game | Lower Bowl Mid | 141 | 2026-09-27 | 9 | LIMITED | NONE | 4.4 | HIGH | Raised in last week; supports increase. |
| COMP-3017 | EVT-1008 | GateLine Resale Marketplace | Rivalry Game | Lower Bowl Mid | 155 | 2026-09-19 | 8 | LIMITED | NONE | 8.0 | STALE | Resale premium; observation is 10 days old. |
| COMP-3018 | EVT-1008 | Larkspur Wolves (home game) | Rivalry Game | Lower Bowl Mid | 118 | 2026-09-28 | 8 | MODERATE | ACTIVE_PROMO | -10.0 | LOW | Bundle promo including parking; not a price comparison. |
| COMP-3019 | EVT-1009 | Larkspur Wolves (home game) | Regular Season Game | Upper Bowl | 39 | 2026-09-27 | 5 | ABUNDANT | NONE | -7.1 | MEDIUM | Lowered late; supports decrease direction. |
| COMP-3020 | EVT-1009 | Ridgeway Live | Regular Season Game | Upper Bowl | 41 | 2026-09-26 | 4 | ABUNDANT | NONE | -2.4 | HIGH | Small decrease. |
| COMP-3021 | EVT-1010 | Marquette Metro Arena | Concert | Lower Bowl Mid | 118 | 2026-09-26 | 31 | MODERATE | NONE | 5.4 | HIGH | Comparable headline concert; raising. |
| COMP-3022 | EVT-1010 | Ridgeway Live | Concert | Lower Bowl Mid | 112 | 2026-09-23 | 25 | LIMITED | NONE | 3.0 | MEDIUM | Smaller act; loosely comparable. |
| COMP-3023 | EVT-1011 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 122 | 2026-09-20 | 16 | MODERATE | NONE | 1.7 | STALE | 9 days old. |
| COMP-3024 | EVT-1011 | Larkspur Wolves (home game) | Regular Season Game | Lower Bowl Mid | 121 | 2026-09-18 | 15 | MODERATE | UNKNOWN |  | STALE | 11 days old; low reliability. |
| COMP-3025 | EVT-1012 | Larkspur Wolves (home game) | Exhibition Game | General Admission | 34 | 2026-09-27 | 10 | MODERATE | NONE | 0.0 | MEDIUM | Exhibition comparable; flat. |
| COMP-3026 | EVT-1013 | Cedar Vale Comets (home game) | Rivalry Game | Lower Bowl Mid | 172 | 2026-09-28 | 4 | LIMITED | NONE | 6.0 | HIGH | Nearly sold out; raising. |
| COMP-3027 | EVT-1013 | GateLine Resale Marketplace | Rivalry Game | Lower Bowl Mid | 205 | 2026-09-28 | 3 | LIMITED | NONE | 9.0 | MEDIUM | Resale premium ~37% over face; secondary market, not a primary comparable. |
| COMP-3028 | EVT-1015 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 110 | 2026-09-27 | 14 | MODERATE | NONE | -6.8 | MEDIUM | Competitor lowered; consistent with softening demand. |
| COMP-3029 | EVT-1015 | GateLine Resale Marketplace | Regular Season Game | Lower Bowl Mid | 101 | 2026-09-28 | 13 | ABUNDANT | ACTIVE_PROMO | -15.0 | LOW | Resale flash discount tied to injury news; volatile. |
| COMP-3030 | EVT-1017 | Larkspur Wolves (home game) | Regular Season Game | Upper Bowl | 62 | 2026-09-26 | 12 | LIMITED | NONE | 3.0 | HIGH | Themed night priced above tier baseline. |
| COMP-3031 | EVT-1018 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 86 | 2026-09-28 | 8 | LIMITED | NONE | 5.0 | HIGH | Competitor raised; near sell-out. |
| COMP-3032 | EVT-1019 | Larkspur Wolves (home game) | Regular Season Game | General Admission | 45 | 2026-09-27 | 17 | MODERATE | NONE | 1.0 | MEDIUM | Kids Day comparable; flat. |
| COMP-3033 | EVT-1020 | Ridgeway Live | Regular Season Game | Club Level | 73 | 2026-09-20 | 54 | LIMITED | NONE | -3.6 | STALE | Auto-generated observation. |
| COMP-3034 | EVT-1020 | Ridgeway Live | Regular Season Game | Club Level | 72 | 2026-09-25 | 55 | MODERATE | NONE | -1.3 | LOW | Auto-generated observation. |
| COMP-3035 | EVT-1021 | GateLine Resale Marketplace | Exhibition Game | Upper Bowl | 36 | 2026-09-16 | 60 | LIMITED | NONE | -0.6 | STALE | Auto-generated observation. |
| COMP-3036 | EVT-1022 | Marquette Metro Arena | Concert | Club Level | 106 | 2026-09-13 | 39 | MODERATE | NONE | -0.2 | STALE | Auto-generated observation. |
| COMP-3037 | EVT-1022 | GateLine Resale Marketplace | Concert | Upper Bowl | 111 | 2026-09-27 | 37 | MODERATE | NONE | 0.8 | LOW | Auto-generated observation. |
| COMP-3038 | EVT-1023 | Marquette Metro Arena | Rivalry Game | Upper Bowl | 126 | 2026-09-28 | 8 | LIMITED | NONE | -0.8 | HIGH | Auto-generated observation. |
| COMP-3039 | EVT-1023 | Cedar Vale Comets (home game) | Rivalry Game | Lower Bowl Mid | 129 | 2026-09-20 | 13 | LIMITED | NONE | 4.3 | STALE | Auto-generated observation. |
| COMP-3040 | EVT-1023 | Larkspur Wolves (home game) | Rivalry Game | Upper Bowl | 120 | 2026-09-20 | 8 | MODERATE | NONE | -2.9 | STALE | Auto-generated observation. |
| COMP-3041 | EVT-1025 | Marquette Metro Arena | Exhibition Game | Club Level | 33 | 2026-09-20 | 6 | ABUNDANT | NONE | 2.8 | STALE | Auto-generated observation. |
| COMP-3042 | EVT-1025 | Larkspur Wolves (home game) | Exhibition Game | Club Level | 37 | 2026-09-16 | 4 | ABUNDANT | NONE | 3.4 | STALE | Auto-generated observation. |
| COMP-3043 | EVT-1025 | Cedar Vale Comets (home game) | Exhibition Game | General Admission | 34 | 2026-09-23 | 9 | LIMITED | NONE | 2.5 | LOW | Auto-generated observation. |
| COMP-3044 | EVT-1026 | GateLine Resale Marketplace | Exhibition Game | Upper Bowl | 34 | 2026-09-27 | 36 | MODERATE | NONE | -1.8 | MEDIUM | Auto-generated observation. |
| COMP-3045 | EVT-1026 | GateLine Resale Marketplace | Exhibition Game | Lower Bowl Mid | 39 | 2026-09-27 | 30 | MODERATE | NONE | -4.1 | LOW | Auto-generated observation. |
| COMP-3046 | EVT-1028 | Larkspur Wolves (home game) | Regular Season Game | Upper Bowl | 72 | 2026-09-25 | 53 | MODERATE | NONE | 1.1 | LOW | Auto-generated observation. |
| COMP-3047 | EVT-1028 | Ridgeway Live | Regular Season Game | General Admission | 66 | 2026-09-16 | 56 | LIMITED | NONE | 3.7 | STALE | Auto-generated observation. |
| COMP-3048 | EVT-1033 | Marquette Metro Arena | Community Night | General Admission | 25 | 2026-09-26 | 35 | LIMITED | NONE | -3.1 | HIGH | Auto-generated observation. |
| COMP-3049 | EVT-1033 | Larkspur Wolves (home game) | Community Night | General Admission | 21 | 2026-09-16 | 36 | ABUNDANT | ACTIVE_PROMO | 9.3 | STALE | Auto-generated observation. Promotion active; temporary. |
| COMP-3050 | EVT-1036 | GateLine Resale Marketplace | Regular Season Game | Club Level | 61 | 2026-09-26 | 15 | MODERATE | ACTIVE_PROMO | 3.3 | LOW | Auto-generated observation. Promotion active; temporary. |
| COMP-3051 | EVT-1036 | Marquette Metro Arena | Regular Season Game | Club Level | 83 | 2026-09-28 | 16 | LIMITED | NONE | 5.0 | LOW | Auto-generated observation. |
| COMP-3052 | EVT-1038 | GateLine Resale Marketplace | Concert | Upper Bowl | 106 | 2026-09-13 | 56 | MODERATE | NONE | 8.1 | STALE | Auto-generated observation. |
| COMP-3053 | EVT-1038 | Ridgeway Live | Concert | General Admission | 124 | 2026-09-28 | 61 | MODERATE | NONE | 1.6 | HIGH | Auto-generated observation. |
| COMP-3054 | EVT-1038 | Ridgeway Live | Concert | Club Level | 115 | 2026-09-13 | 62 | MODERATE | NONE | -0.4 | STALE | Auto-generated observation. |
| COMP-3055 | EVT-1039 | Ridgeway Live | Regular Season Game | Club Level | 87 | 2026-09-26 | 1 | LIMITED | NONE | -0.9 | MEDIUM | Auto-generated observation. |
| COMP-3056 | EVT-1040 | Marquette Metro Arena | Regular Season Game | General Admission | 41 | 2026-09-26 | 8 | MODERATE | NONE | 2.0 | MEDIUM | Auto-generated observation. |
| COMP-3057 | EVT-1040 | Ridgeway Live | Regular Season Game | Club Level | 46 | 2026-09-25 | 8 | MODERATE | NONE | -3.0 | MEDIUM | Auto-generated observation. |
| COMP-3058 | EVT-1041 | Marquette Metro Arena | Regular Season Game | Club Level | 88 | 2026-09-13 | 56 | MODERATE | NONE | 2.9 | STALE | Auto-generated observation. |
| COMP-3059 | EVT-1041 | Ridgeway Live | Regular Season Game | Upper Bowl | 82 | 2026-09-13 | 62 | MODERATE | NONE | -0.9 | STALE | Auto-generated observation. |
| COMP-3060 | EVT-1041 | Ridgeway Live | Regular Season Game | General Admission | 69 | 2026-09-13 | 59 | ABUNDANT | ACTIVE_PROMO | 4.7 | STALE | Auto-generated observation. Promotion active; temporary. |
| COMP-3061 | EVT-1042 | Larkspur Wolves (home game) | Regular Season Game | General Admission | 44 | 2026-09-25 | 14 | MODERATE | NONE | 11.3 | HIGH | Auto-generated observation. |
| COMP-3062 | EVT-1043 | Larkspur Wolves (home game) | Regular Season Game | Club Level | 88 | 2026-09-23 | 29 | LIMITED | NONE | -1.7 | LOW | Auto-generated observation. |
| COMP-3063 | EVT-1043 | GateLine Resale Marketplace | Regular Season Game | Lower Bowl Mid | 82 | 2026-09-20 | 35 | LIMITED | NONE | -1.4 | STALE | Auto-generated observation. |
| COMP-3064 | EVT-1044 | Cedar Vale Comets (home game) | Exhibition Game | Upper Bowl | 34 | 2026-09-16 | 29 | MODERATE | NONE | 1.1 | STALE | Auto-generated observation. |
| COMP-3065 | EVT-1045 | Marquette Metro Arena | Exhibition Game | Club Level | 37 | 2026-09-20 | 23 | MODERATE | NONE | -6.9 | STALE | Auto-generated observation. |
| COMP-3066 | EVT-1045 | Larkspur Wolves (home game) | Exhibition Game | Upper Bowl | 37 | 2026-09-20 | 29 | MODERATE | NONE | 5.3 | STALE | Auto-generated observation. |
| COMP-3067 | EVT-1048 | Cedar Vale Comets (home game) | Regular Season Game | Lower Bowl Mid | 43 | 2026-09-13 | 49 | MODERATE | NONE | -7.0 | STALE | Auto-generated observation. |
| COMP-3068 | EVT-1048 | Ridgeway Live | Regular Season Game | Club Level | 47 | 2026-09-23 | 47 | LIMITED | NONE | -0.4 | HIGH | Auto-generated observation. |
| COMP-3069 | EVT-1049 | Larkspur Wolves (home game) | Community Night | General Admission | 30 | 2026-09-25 | 56 | LIMITED | NONE | -0.4 | LOW | Auto-generated observation. |
| COMP-3070 | EVT-1049 | GateLine Resale Marketplace | Community Night | General Admission | 25 | 2026-09-23 | 55 | MODERATE | ACTIVE_PROMO | 3.0 | LOW | Auto-generated observation. Promotion active; temporary. |
| COMP-3071 | EVT-1050 | Larkspur Wolves (home game) | Regular Season Game | General Admission | 73 | 2026-09-20 | 6 | MODERATE | ACTIVE_PROMO | 7.4 | STALE | Auto-generated observation. Promotion active; temporary. |
| COMP-3072 | EVT-1050 | GateLine Resale Marketplace | Regular Season Game | Lower Bowl Mid | 74 | 2026-09-13 | 9 | MODERATE | ACTIVE_PROMO | 6.1 | STALE | Auto-generated observation. Promotion active; temporary. |
| COMP-3073 | EVT-1050 | Marquette Metro Arena | Regular Season Game | Club Level | 88 | 2026-09-25 | 3 | LIMITED | NONE | 6.1 | MEDIUM | Auto-generated observation. |

## 4. Pricing Policy and Guardrails

### Harborlight Sports & Entertainment (Fictional): Dynamic Pricing Policy and Guardrails

Document ID: SRC-04 | Version: 3.2 (synthetic) | Effective date: 2026-07-01 | Synthetic as-of date for this knowledge base: 2026-09-29 Policy owner: VP, Revenue Management & Pricing Governance | Approved by: Pricing Governance Committee | Review cycle: Quarterly

Authority. This document is authoritative for all price guardrails. Where it conflicts with an ML output, a competitor observation, a historical analog, or a revenue-maximizing argument, this policy prevails. Only a human pricing decision-maker with the authority named in P-16 may approve an exception. PricePilot cannot grant exceptions.

Rule IDs (P-01 to P-19) are stable so recommendations can cite them.

### P-01 Scope and definitions

Price basis. current_price is the event's reference-section ticket price. All bounds and percentage limits apply to this price. average_ticket_price is a realized blended price and is informational only.

Percent change = (recommended price − current_price) ÷ current_price. Recommended prices are whole dollars. When a limit produces a fractional price, round down for increases and up for decreases so the limit is never exceeded.

Remaining inventory % = available_inventory ÷ venue_capacity. held_inventory (sponsor/comp/production holds) is excluded from both sold and available.

Sell-through states: Critical Scarcity ≥ 95% sold; High 85–94.9%; Healthy 60–84.9%; Soft 40–59.9%; Weak < 40%.

Velocity ratio = sales_velocity_3d ÷ sales_velocity_7d. Accelerating > 1.10; Steady 0.90–1.10; Decelerating < 0.90. The sales_velocity_trend label is a convenience. If the label conflicts with the numbers, the numbers govern and the conflict must be reported.

Sales curves are back-loaded. A low sold % well before the event, by itself, is not evidence of weak demand (see P-07).

### P-02 Price bounds by event tier

| Tier | Description | Minimum reference price | Maximum reference price |
|---|---|---:|---:|
| A | Marquee (playoffs, top rivalries, marquee openers) | $85 | $320 |
| B | Premium | $55 | $210 |
| C | Standard | $35 | $120 |
| D | Value | $22 | $75 |

A recommendation outside these bounds is invalid. PricePilot must clamp to the bound and escalate (P-16). Revenue upside never justifies exceeding a bound.

Any increase producing a price at or above 95% of the tier maximum requires human review (P-05).

### P-03 Maximum change in a single recommendation

| Tier | Max increase | Max decrease |
|---|---:|---:|
| A | +10% | −8% |
| B | +12% | −10% |
| C | +12% | −10% |
| D | +15% | −10% |

These are ceilings, not targets. Other rules frequently set lower ceilings; the most restrictive applicable limit governs.

### P-04 Rolling 14-day cumulative limit

The net change relative to the price in effect 14 days earlier may not exceed ±25%. Use last_price_change_pct and days_since_last_price_change where the last change falls within 14 days. If the cumulative limit would be breached, reduce the recommendation to fit and flag it.

### P-05 Price increase review triggers

An increase requires additional human review (recommendation must be labeled "Review Required") if any apply:

- Single-recommendation increase greater than 8%.
- Resulting price is ≥ 95% of the tier maximum.
- Increase greater than 5% while remaining inventory exceeds 40% (P-06).
- Increase greater than 5% when no valid competitor data exists (P-12).
- Decelerating velocity, low/missing ML confidence, volatility, or unresolved conflicting evidence apply (P-07, P-11, P-13, P-14).
- The event is strategic (P-17).

### P-06 Inventory thresholds

| Remaining inventory | Meaning | Rule |
|---|---|---|
| < 8% | Limited Availability | Increases up to the P-03 cap are allowed; tier-max and review rules still apply. |
| 8–40% | Normal | No inventory-based restriction. |
| > 40% | Ample | Increases are capped at +5% regardless of demand signals. Above 5% requires review and a written justification. Strong velocity does not override this cap because large remaining inventory carries sell-through risk. |
| 0 | Sold out | HOLD (P-15). |

If available_inventory and capacity-based remaining inventory disagree such that P-06 could be triggered under one figure and not the other, treat as a data conflict (P-13, P-15).

### P-07 Sell-through and sales-velocity thresholds

Strong demand signal: sold ≥ 85%, or forecast ≥ 95% with velocity not decelerating.

Soft (40–59.9% sold) with more than 10 days remaining is not, by itself, grounds for a decrease. Default is HOLD and monitor, particularly for Rivalry, Playoff and Season Opener events.

Increases when velocity is Decelerating (ratio < 0.90) and sold < 95% are capped at +4% and require review.

Missing sales_velocity_7d: no increase may be recommended (HOLD), and a data-quality escalation is required.

A demand forecast must never be treated as certain. Forecast confidence below 0.60 requires review for any change.

### P-08 Minimum interval between price changes (cooling-off)

A price change may not be recommended if the last change was fewer than 7 days ago (days_since_last_price_change < 7). This applies even when demand is exceptionally strong. It protects price integrity and customer trust and deliberately sacrifices some revenue. Only Pricing Leadership may waive it (P-16).

### P-09 Final 72 hours

Within 3 days of the event, increases are not permitted unless sold ≥ 95%. Any decrease within 3 days requires human review.

### P-10 Price decrease rules

A decrease may be recommended only if all of the following hold: (a) days to event ≤ 14; (b) sold < 50%; (c) demand forecast < 80%; (d) velocity is not Accelerating; (e) event is not strategic.

Additional rules:

- Decreases greater than 5% require review.
- Protected events (Tier A or B Rivalry, Playoff, Season Opener) require review for any decrease. The default is to protect price integrity.
- Decreases within 72 hours require review.
- No decreases when sold ≥ 85%.
- Historical evidence showing that a discount did not lift demand for a comparable situation must be weighed and disclosed.

### P-11 ML confidence rules

| ML_model_confidence | Treatment |
|---|---|
| ≥ 0.75 | High. ML output may be weighted heavily but never overrides policy. |
| 0.60–0.74 | Medium. Corroborate with at least one independent source before acting. |
| 0.45–0.59 | Low. Recommended change capped at ±5%, review required if above 3%. |
| < 0.45 | Very low. HOLD and escalate. |
| Missing | Treated as Unknown-Low: change capped at ±3% with review, and the gap must be stated. PricePilot must never assume a confidence value. |

demand_forecast_confidence below 0.60 independently requires review for any change. Missing price_elasticity_estimate must be stated as a limitation; do not infer a value.

### P-12 Competitor data rules

Competitor pricing is context, never a mandate. It may not be the sole basis for a change, and PricePilot must not price-match automatically or treat competitor prices as floors or ceilings.

Stale: observations older than 7 days may not justify a change (context only). Older than 21 days: disregard except to note it exists.

Promotions: records with a non-"No Promotion" status (Flash Sale, Bundle Promotion, Group Discount) are excluded from baseline comparisons.

Records with data_quality of Low, Missing or Stale are excluded from price comparisons.

Missing competitor data does not block action but must be disclosed. Increases above 5% require review when no valid competitor data exists.

Competitor price gaps must be interpreted against the competitor's inventory signal and demand profile. A persistently lower price on a weaker event is structural and not a reason to follow.

### P-13 Conflicting evidence

Evidence sources: ML recommendation, current sell-through/velocity/inventory, historical analogs, valid competitor data.

If the ML direction conflicts with two or more of the other sources, do not adopt the ML price. Recommend HOLD or a reduced change, mark "Review Required," and explain the conflict.

If ML conflicts with a highly comparable historical analog (same event type and tier; same venue or capacity band; days within ±5; sold % within ±8 pts), limit the change to no more than half the ML change and flag it.

A "closest" historical row is not automatically comparable. Momentum (velocity trend), tier and venue matter (see knowledge-base governance).

Conflicting input fields (e.g., trend label vs velocity numbers; inventory that does not sum to capacity) must be reported. PricePilot must not silently choose one.

### P-14 Volatile events

An event is volatile if |forecast_change_vs_prior_week| > 25 points. For volatile events: HOLD unless a human approves; any change PricePilot suggests is limited to ±3% pending review; the cause of the swing must be requested if unknown.

### P-15 Conditions requiring HOLD / NO CHANGE

PricePilot must recommend HOLD when any of the following is true:

- Sold out or available_inventory = 0.
- event_status is Postponed, Cancelled or Suspended, or otherwise not On Sale/Limited Availability.
- Last price change < 7 days ago (P-08).
- ML_model_confidence < 0.45 (P-11).
- sales_velocity_7d missing and the proposed action is an increase (P-07).
- Unresolved inventory inconsistency exceeding 2% of capacity.
- Volatile event without human approval (P-14).
- The only support for a change is stale, promotional, or low-quality competitor data.
- Evidence is genuinely balanced and no eligibility rule for change is met.

HOLD is a valid, complete recommendation. It must still be explained.

### P-16 Mandatory escalation to a human

PricePilot must explicitly escalate (state that human review is required, why, and what decision is needed) when: an ML recommendation would breach P-02, P-03, P-04, P-08, P-09, P-10 or P-17; a change is at or above a review trigger; data conflicts remain unresolved; any Mandatory HOLD in P-15 applies (data or status related); event is volatile or strategic.

| Decision | Authority |
|---|---|
| Changes labeled "Review Required" | Director, Pricing & Yield |
| Exceptions to P-08 (cooling-off), P-09, P-10 protected events, P-17 | VP, Revenue Management & Pricing Governance |
| Any price outside P-02 bounds | Pricing Governance Committee |

### P-17 Strategic / community events

For events with strategic_flag = Y (e.g., Community Night): increases capped at +5%; no decreases without VP approval; goodwill and access objectives outrank revenue. Historical evidence of backlash (HST-2028) is on record.

### P-18 Rules that deliberately override revenue maximization

The following apply even when the model or a revenue estimate indicates a higher-revenue alternative:

- Cooling-off (P-08). No change < 7 days after the last change, even on a sellout trajectory.
- Strategic cap (P-17). Community events do not chase the market.
- Tier maximums (P-02). A sellout event stops at the tier ceiling.
- Large-inventory cap (P-06). Strong velocity does not justify large increases when > 40% of capacity remains.
- Protected-event decreases (P-10). Price integrity outranks a modeled sell-through gain.
- Late-window integrity (P-09). No last-minute increases on sub-95% sold events.

### P-19 Output requirements for recommendations

Every PricePilot recommendation must state: action, exact price, percent change, the binding rule(s), evidence used with source IDs (event ID, comparable IDs, competitor record IDs, policy rule IDs), conflicts and uncertainty, missing data, whether review is required and by whom, and that the final decision rests with the human pricing decision-maker. PricePilot must not invent missing values.

## 5. Data Relationships

- Use `event_id` to connect event-level records in **Event Pricing Inputs and ML Outputs** with related competitor or secondary-market records in **Competitor / Secondary Market Pricing**.
- Use `comparable_event_id` in the event-level dataset to connect an event to the corresponding `comparable_event_id` in **Historical Comparable Events**.
- Use `competitor_event_id` to identify individual competitor or secondary-market observations within the competitor-pricing dataset.
- Event type, event tier, venue capacity, days to event, sold percentage, and related named fields are present in more than one dataset and can be compared where applicable; they do not replace the identifier-based connections above.
- Policy rule IDs `P-01` through `P-19` identify constraints in **Pricing Policy and Guardrails** that may be referenced alongside event, historical, and competitor records.

## 6. Data Usage Instructions

Treat this as synthetic testing data.

Use the Event ID as the primary identifier when connecting event-level information across datasets.

When analyzing an event, use all relevant available information rather than relying on a single variable.

ML outputs are model inputs/evidence, not guaranteed facts or automatically correct recommendations.

Historical events are evidence for comparison, not deterministic precedents.

Competitor/secondary-market prices are contextual market signals, not instructions to automatically match market prices.

Pricing policies and guardrails should be treated as constraints when making recommendations.

If required information is missing, do not invent it.

If data sources conflict, identify the conflict rather than silently choosing one.

This file is for AI analysis and testing; it does not authorize automatic price changes.
