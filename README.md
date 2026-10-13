# IRONBOUND Aerospace

Twelve approved Inner Sphere aerospace fighter records for the IRONBOUND campaign. Each SVG is 277 × 183 mm and fits the existing Homebrewery unitRecordPage wrapper.

## Files

- `IRONBOUND-*.svg`: printable vector records.
- `IRONBOUND-Aerospace-Cards.md`: complete copyable Homebrewery insertion block, catalogue values and upkeep addition.
- `profiles.json`: converted values, weapon TICs, ammunition bins and source paths.

## Sources and conversion

Stock construction data: [MegaMek mm-data](https://github.com/MegaMek/mm-data/tree/main/data/mekfiles/fighters). Published baseline BV2 and catalogue prices: [Master Unit List](https://masterunitlist.info/). Conversion: supplied BattleTech Override v5.3r1 and MechWarrior: Destiny. Fighter silhouette and hit-location layout follow the supplied Override fighter diagram. Campaign heat, crew and operating costs follow IRONBOUND.

Armor is Classic armor / 4, normal half-up rounding. Shared Structure is SI / 3 with a minimum of 1. Standard fighter SI = max(floor(tonnage / 10), Safe Thrust), confirmed in [MegaMek Aero.autoSetSI](https://github.com/MegaMek/megamek/blob/main/megamek/src/megamek/common/units/Aero.java). DThr is (Classic Nose + Aft + one Wing armor) / 30, normal rounding. Dissipation is single heat sinks / 5, normal rounding. Airborne TMM includes the flying modifier. Bomb capacity uses Alpha Strike BOMB values (1/2/3 by these fighters’ size).

TICs contain all stock weapons, with base damage at most 5 and max damage at most 14. Each printed ammo row represents one original fuselage bin. Identical single wing weapons can share a TIC; rear weapons remain separate. Weapons destroyed in a TIC disable that entire TIC.

EV adopts published BV2 as a campaign reference at G4/P5, rather than claiming a separately calibrated Override rating. CV was checked against the standard fusion fighter construction calculation: cockpit, life support, sensors, SI, flight systems, engine, fuel tanks, armor, heat sinks, weapons and ammo, then the tonnage multiplier. [Calculation source](https://github.com/MegaMek/megamek/blob/main/megamek/src/megamek/common/cost/AeroCostCalculator.java). The Thunderbird uses 6,430,500 C-bills, matching the current MUL and construction calculation.

Upkeep: 20 C-bills/ton/day, fighter only. Regular pilot wages: 700/day, separate; hiring: 30,000. Bombs, repairs, ammo, travel and transport are additional.

## Validation

All 12 SVGs were parsed and rendered. Checked every weapon mount against stock data, legal TIC limits, bin counts and shots, stock cost calculation, converted armor and structure, and exact pip counts in all five tracks. Layout checked on rendered records, including the eight-TIC Chippewa and Stuka.

Fan-made campaign aids; BattleTech and its related marks belong to their respective owners.
