# Kapittel 6 – Momentumanalyse av strømsystemer

## Lineær momentumlikning (kontrollvolum)

Fra RTT med $b = \vec{V}$:

> $\sum \vec{F} = \frac{d}{dt}\int_{KV} \rho \vec{V} \, dV + \int_{KF} \rho \vec{V} \, (\vec{V} \cdot \hat{n}) \, dA$

For **stasjonær** strøm:

> $\sum \vec{F} = \sum_{ut} \dot{m} \vec{V} - \sum_{inn} \dot{m} \vec{V}$

$\sum \vec{F}$ inkluderer: trykkkrefter, tyngdekraft, reaksjonskraft fra vegger/rør.

---

## Fremgangsmåte

1. Tegn kontrollvolum og merk alle krefter på det
2. Velg koordinatsystem (positiv retning)
3. Skriv opp $x$- og $y$-komponentene separat
4. Løs for ukjent kraft

**Konvensjon:** $\vec{V} \cdot \hat{n} > 0$ ved utstrøm, $< 0$ ved innstrøm

---

## Typiske anvendelser

### Rørbow (bend)
Fluid endrer retning → veggen må levere en kraft.

For stasjonær inkompressibel strøm ($\dot{m}_1 = \dot{m}_2 = \dot{m}$):

> $F_x = \dot{m}(V_{2x} - V_{1x}) + (P_2 A_2)_x - (P_1 A_1)_x$

Kraften fra røret på fluidet er $\vec{F}_R$; reaksjonskraft på røret er $-\vec{F}_R$.

### Dyse (nozzle)
Trykk omdannes til hastighet. Normalt: $P_{utløp} = P_{atm}$

### Jetimpuls mot plate
Fluid treffer stasjonær plate:

> $F = \dot{m}(V_{ut} - V_{inn})$

For normalt innfall og fri spredning: $F = \rho A V^2$

---

## Manometer og trykkmåling

Brukes for å finne trykk i rørstrøm. Kombiner med energiligningen for å finne tap eller hastighet.
