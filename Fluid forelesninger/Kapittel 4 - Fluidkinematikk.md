# Kapittel 4 – Fluidkinematikk

## Beskrivelsesmetoder

**Lagrangisk** – følger én bestemt fluidpartikkel over tid (som å feste en GPS på partikkelen)  
**Euleriansk** – beskriver felt i faste punkter i rommet; dette brukes i fluid-mekanikk

---

## Strømlinje, banesport og strekstrie

**Strømlinje** – kurve som til enhver tid er tangent til hastighetsvektoren. I stasjonær strøm sammenfaller alle tre.

> Ingen strømning kan krysse en strømlinje

**Banesport (pathline)** – banen én partikkel faktisk følger over tid  
**Strekstrie (streakline)** – linje som forbinder alle partikler som har passert et gitt punkt (f.eks. fargestoffinjeksjon)

I **stasjonær strøm**: strømlinje = banesport = strekstrie

---

## Materiell derivert

Akselerasjonen til en fluidpartikkel (Lagrangiansk) uttrykt med Eulerianske felt:

> $\frac{D\vec{V}}{Dt} = \underbrace{\frac{\partial \vec{V}}{\partial t}}_{\text{lokal}} + \underbrace{(\vec{V} \cdot \nabla)\vec{V}}_{\text{konvektiv}}$

- **Lokal** akselerasjon: endring over tid i et fast punkt
- **Konvektiv** akselerasjon: endring fordi partikkelen beveger seg til et sted med annen hastighet

I **stasjonær strøm**: $\partial \vec{V}/\partial t = 0$, men konvektiv akselerasjon kan fortsatt være $\neq 0$

---

## Reynolds Transport Theorem (RTT)

Kobling mellom systemet (Lagrangiansk) og kontrollvolumet (Euleriansk):

> $\frac{dB_{sys}}{dt} = \frac{d}{dt}\int_{KV} \rho b \, dV + \int_{KF} \rho b \, (\vec{V} \cdot \hat{n}) \, dA$

der $B$ er en vilkårlig ekstensiv størrelse og $b = B/m$ er den intensive ekvivalenten.

Brukes til å utlede kontinuitets-, moment- og energilikningen for kontrollvolum.

---

## Strøm-klassifisering

| Egenskap | Beskrivelse |
|---|---|
| Stasjonær | $\partial/\partial t = 0$ — felt endrer seg ikke over tid |
| Uniform | $\partial/\partial s = 0$ — felt endrer seg ikke i rommet |
| Inkompressibel | $\rho = \text{konst}$ |
| 1D / 2D / 3D | Antall romlige koordinater som trengs |

**Strømlinjekordinat:** $s$ langs strømlinje, $n$ normalt. Akselerasjon langs strømlinje:

> $a_s = V\frac{\partial V}{\partial s}$ (konvektiv) $\qquad a_n = \frac{V^2}{R}$ (sentripetal, mot sentrum av krumning)
