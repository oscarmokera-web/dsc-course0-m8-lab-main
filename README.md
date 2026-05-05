# Aviation Accident Safety Analysis

## What we did

We looked at aviation accident data from 1948 to 2023, but focused on 1983 onwards (assuming planes older than 40 years aren't really active anymore). The client – an airline insurer – wanted to know which aircraft makes/models are least likely to get destroyed or seriously hurt passengers when something goes wrong. They also wanted separate advice for small planes (≤20 seats) and larger passenger jets.

## How we cleaned the mess

The raw data was... messy. We:
- Converted dates and filtered to 1983+
- Created a “injury fraction” – basically, out of everyone on board, how many died or were seriously hurt
- Flagged which accidents destroyed the aircraft
- Standardised manufacturer names (Boeing is Boeing, not "THE BOEING COMPANY")
- Kept only makes and models with enough accidents to be statistically meaningful (at least 10 incidents)

## What we found (the good stuff)

### Safest aircraft makes – quick look

| Size | Top makes | Injury rate | How often destroyed |
|------|-----------|-------------|---------------------|
| Large (jets) | Boeing, Airbus, Bombardier | 2-4% | 15-22% |
| Small | Cessna, Piper, Beechcraft | 6-9% | 31-45% |

Bottom line: large jets are way safer for passengers – only 2-4% of people on board get seriously hurt in an accident. Small planes are riskier, but some are still better than others.

### Specific models we'd recommend

**Large planes:**
- Boeing 737-800
- Airbus A320 family
- Bombardier CRJ series

**Small planes:**
- Cessna 172 (the classic)
- Piper PA-28
- Beechcraft Bonanza

These consistently came out on top with low injury rates and reasonable destruction rates.

## Two factors that really matter

### 1. Weather

Bad weather (IMC – clouds, low visibility) makes accidents much worse. Injury rate jumps from 27% (good weather) to 41% (bad weather). Planes also get destroyed more often. So maybe charge more for flights in poor conditions or require instrument-rated pilots.

### 2. Phase of flight

Cruise accidents are rare but brutal – 68% of people on board get seriously hurt. Landing accidents happen more often but are less deadly (22% injury rate). Takeoff and approach sit in the middle. Not much you can do about cruise phase, but good training for takeoff/landing could help.

## Our recommendations

**For large aircraft** – insure Boeing, Airbus, Bombardier. Avoid older or obscure models with little track record.

**For small aircraft** – Cessna, Piper, Beechcraft are your best bets. But expect higher claims rates than jets – price accordingly.

**Underwriting tips** – consider weather clauses and pilot training requirements. Cruise accidents are scary but rare; focus on the more common (and survivable) landing incidents.

## What we couldn't do

We didn't have pilot experience, maintenance records, or flight hours. Those probably matter too. Also, some models had so few accidents that our stats aren't rock solid – keep an eye on them.

## Files in this repo

- `Aviation_Accidents_Cleaning.ipynb` – all the messy cleaning code
- `Aviation_Accidents_Data_Analysis.ipynb` – the analysis and pretty charts
- `README.md` – this summary

## Want to rerun this?

1. Grab the data from [Kaggle](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database)
2. Run the cleaning notebook first, then the analysis notebook
3. You'll get the same numbers and plots

---

*– Your friendly aviation data consultancy*