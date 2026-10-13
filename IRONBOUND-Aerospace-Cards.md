# IRONBOUND — Aerospace Cards

Die zwölf Karten sind jeweils eine vollständige Druckseite im vorhandenen `unitRecordPage`-Layout. Es ist keine zusätzliche CSS-Anpassung nötig.

**Einfügen:** In IRONBOUND — Unit Records nach der letzten Vehicle-Karte und vor dem Pilot Directory. Falls Vehicles noch nicht eingefügt sind, nach der letzten BattleMech-Karte. Der folgende Block beginnt auf einer neuen Seite und endet mit einem Seitenwechsel für den bestehenden nächsten Abschnitt.

```md
\page

{{unitRecordPage
![Cheetah F-10](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Cheetah-F-10.svg)
}}

\page

{{unitRecordPage
![Chippewa CHP-W5](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Chippewa-CHP-W5.svg)
}}

\page

{{unitRecordPage
![Corsair CSR-V12](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Corsair-CSR-V12.svg)
}}

\page

{{unitRecordPage
![Lucifer LCF-R15](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Lucifer-LCF-R15.svg)
}}

\page

{{unitRecordPage
![Seydlitz SYD-21](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Seydlitz-SYD-21.svg)
}}

\page

{{unitRecordPage
![Shilone SL-17](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Shilone-SL-17.svg)
}}

\page

{{unitRecordPage
![Sholagar SL-21](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Sholagar-SL-21.svg)
}}

\page

{{unitRecordPage
![Slayer SL-15](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Slayer-SL-15.svg)
}}

\page

{{unitRecordPage
![Sparrowhawk SPR-H5](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Sparrowhawk-SPR-H5.svg)
}}

\page

{{unitRecordPage
![Stingray F-90](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Stingray-F-90.svg)
}}

\page

{{unitRecordPage
![Stuka STU-K5](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Stuka-STU-K5.svg)
}}

\page

{{unitRecordPage
![Thunderbird TRB-D36](https://raw.githubusercontent.com/helmutlukasczyk-coder/ironbound-aerospace/main/IRONBOUND-Thunderbird-TRB-D36.svg)
}}

\page
```

## Katalogübersicht

| Fighter | Jahr | t | EV | CV / C-bills | Unterhalt / Tag |
|:--|--:|--:|--:|--:|--:|
| Cheetah F-10 | 2630 | 25 | 448 | 1,669,463 | 500 |
| Chippewa CHP-W5 | 2584 | 90 | 1520 | 5,410,530 | 1,800 |
| Corsair CSR-V12 | 2779 | 50 | 1190 | 2,293,958 | 1,000 |
| Lucifer LCF-R15 | 2526 | 65 | 1329 | 3,162,311 | 1,300 |
| Seydlitz SYD-21 | 2504 | 20 | 440 | 1,370,380 | 400 |
| Shilone SL-17 | 2796 | 65 | 1230 | 3,399,045 | 1,300 |
| Sholagar SL-21 | 2803 | 35 | 607 | 2,052,353 | 700 |
| Slayer SL-15 | 2770 | 80 | 1288 | 4,454,053 | 1,600 |
| Sparrowhawk SPR-H5 | 2520 | 30 | 637 | 1,740,870 | 600 |
| Stingray F-90 | 2762 | 60 | 1268 | 2,979,080 | 1,200 |
| Stuka STU-K5 | 2571 | 100 | 1790 | 6,156,000 | 2,000 |
| Thunderbird TRB-D36 | 2480 | 100 | 1932 | 6,430,500 | 2,000 |

## Ergänzung für das Hauptregelwerk

Unter **Company Aerospace Support → Purchasing and Maintaining Fighters**, nach dem Absatz zu täglichen Betriebskosten, ergänzen:

```md
Aerospace fighter upkeep is **20 C-bills per ton per campaign day**. This covers the fighter only; charge pilot wages separately. A regular aerospace pilot costs **700 C-bills per day** under the hiring rules. Ammunition, bombs, repairs, and transport remain separate expenses.
```

## Verwendete Werte

- EV entspricht dem veröffentlichten BV2 bei Gunnery 4 / Piloting 5 als IRONBOUND-Katalogreferenz. Die Karten enthalten keine separate neue Override-Punktebewertung.
- Rüstung: Classic-Wert je Zone / 4, normal gerundet. Struktur: Classic-SI / 3, normal gerundet, mindestens 1. Bei diesen Standard-Fightern ist SI der höhere Wert aus Safe Thrust und abgerundeter Tonnage / 10.
- DThr: Classic-Rüstung von Nose + Aft + einer Wing / 30, normal gerundet. Der Wert bleibt fest.
- Trefferdiagramm nach der bereitgestellten Override-Vorlage: Nose 6–8, Right Wing 3–5, Left Wing 9–11, Aft 2 und 12; eine gemeinsame Strukturleiste.
- Alle Originalwaffen und Munitionsbehälter bleiben erhalten. TICs halten Override-Grenzen von Basis 5 und Maximum 14 ein. Die Corsair hat deshalb zwei separate Large-Laser-TICs.
- Wärmeeffekte folgen IRONBOUND: Wärme 1 senkt Current Thrust um 1; der gedruckte TMM wird dadurch nicht reduziert.
- Bombenkapazität nach Alpha Strike: leichte Fighter 1, mittlere 2, schwere 3. Bomben sind keine enthaltene Startladung.
- Katalogpreise sind reine Fighter-Werte. Thunderbird TRB-D36: 6,430,500 C-bills; Seydlitz SYD-21 und Sparrowhawk SPR-H5 sind die hier verwendeten frühen Varianten.
