# P2 · Kisan Query Router — public data (participant-facing)

Real farmer helpline queries (as typed by call-centre advisers) from one Indian state, 2025. Data source not disclosed.

Files
- `train.csv` — 29,512 unique query texts: `id,text,district,month,query_type,crop`.
- `sample_submission.csv` — `id,query_type,crop`.

Labels
- `query_type` (11 classes): schemes_credit_insurance, plant_protection, nutrient_fertilizer, cultural_practices, varieties_seeds, weed_management, water_management, weather_sowing_time, post_harvest_market, animal_husbandry, other.
- `crop` (27 classes): 25 frequent crops + `other_crop` (a specific crop outside the list) + `none_or_general` (no crop, e.g. scheme queries).
- Labels were assigned by call-centre staff: expect some noise. Long digit strings were masked as `[NUMBER]` for privacy.
