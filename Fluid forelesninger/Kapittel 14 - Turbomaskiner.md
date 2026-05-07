# Kapittel 14 – Turbomaskiner

## Klassifisering

| Type | Energioverføring | Eksempler |
|---|---|---|
| Pumpe / vifte / kompressor | Tilføres fra aksel til fluid | Sentrifugalpumpe, aksialvifte |
| Turbin | Tas ut fra fluid til aksel | Pelton, Francis, Kaplan |

**Radial (sentrifugal)** – høyt trykk, lav flow  
**Aksial** – lavt trykk, høy flow  
**Mixed-flow** – kombinasjon

---

## BEP – Best Efficiency Point

BEP er punktet på H-Q kurven der $\eta$ er maksimal. Noteres med $*$: $Q^*$, $H^*$, $\text{bhp}^*$.

**Bremsehestekraft (bhp)** = faktisk akseltilført effekt:

> $\text{bhp} = \frac{\rho g Q H}{\eta_{pumpe}}$

**Virkningsgrad lest av ved BEP:**

> $\eta_{max} = \frac{\rho g Q^* H^*}{\text{bhp}^*}$

Pumper skal velges slik at driftspunktet er nær BEP.

---

## Systemkurve og driftspunkt

Energiligningen mellom reservoar ① og utløp ② (store reservoarer: $V_1 \approx V_2 \approx 0$, $P_1 = P_2 = P_{atm}$):

> $H_{nødvendig} = (z_2 - z_1) + h_L$

der $h_L = \left(f\dfrac{L}{D} + \sum K_L\right)\dfrac{V^2}{2g}$

**Driftspunktet** er der $H_{nødvendig} = H_{nyttbar}$ — tegn systemkurven inn i pumpe-H-Q diagrammet og finn skjæringen.

---

## Kavitasjon og NPSH

**Kavitasjon** oppstår når lokaltrykket faller under $P_v$ → bobler kollapser → støy, erosjon, ytelsesfall.

**NPSH nyttbar** — utled via energiligningen fra reservoaroverflate ① til pumpeinnløp ②:

> $\text{NPSH}_{nyttbar} = \frac{P_{atm} - P_v}{\rho g} + (z_1 - z_2) - h_L$

- $(z_1 - z_2) > 0$: pumpen under reservoar → gunstig
- $(z_1 - z_2) < 0$: pumpen over reservoar → reduserer NPSH

**$\text{NPSH}_{nødvendig}$** leses av fra pumpeytelseskurven ved aktuelt $Q$.

**Krav (med sikkerhetsmargin):**

> $\text{NPSH}_{nyttbar} > 1{,}5 \cdot \text{NPSH}_{nødvendig}$

**Finn maks plassering av pumpe** (sett $z_1 = 0$, løs for $z_2$):

> $z_2 < \frac{P_{atm} - P_v}{\rho g} - h_L - 1{,}5 \cdot \text{NPSH}_{nødvendig}$

Negativ $z_2$ → pumpen må plasseres **under** vannspeilet.

---

## Affinitetslover

Forutsetning: pumper er **dynamisk like** (opererer ved BEP).

### Endre turtall, samme diameter

> $\frac{Q_B}{Q_A} = \frac{\omega_B}{\omega_A} \qquad \frac{H_B}{H_A} = \left(\frac{\omega_B}{\omega_A}\right)^2 \qquad \frac{\text{bhp}_B}{\text{bhp}_A} = \left(\frac{\omega_B}{\omega_A}\right)^3$

**Finn ny $\omega$ for ønsket $H$:**

> $\omega_B = \sqrt{\frac{H_B}{H_A}} \cdot \omega_A$

### Endre diameter, samme turtall

> $\frac{Q_B}{Q_A} = \left(\frac{D_B}{D_A}\right)^3 \qquad \frac{H_B}{H_A} = \left(\frac{D_B}{D_A}\right)^2 \qquad \frac{\text{bhp}_B}{\text{bhp}_A} = \left(\frac{D_B}{D_A}\right)^5$

### Endre både $\omega$ og $D$

> $\frac{Q_B}{Q_A} = \frac{\omega_B}{\omega_A}\left(\frac{D_B}{D_A}\right)^3 \qquad \frac{H_B}{H_A} = \left(\frac{\omega_B}{\omega_A}\right)^2\left(\frac{D_B}{D_A}\right)^2 \qquad \frac{\text{bhp}_B}{\text{bhp}_A} = \frac{\rho_B}{\rho_A}\left(\frac{\omega_B}{\omega_A}\right)^3\left(\frac{D_B}{D_A}\right)^5$

### Virkningsgradsskalering (Moody-formelen)

Større pumpe ($D_B > D_A$) → lavere veggfriksjonstap → høyere $\eta$:

> $\eta_{B,max} = 1 - (1 - \eta_{A,max})\left(\frac{D_A}{D_B}\right)^{1/5}$

---

## Spesifikk turtall $N_{sp}$

Brukes til å identifisere pumpe-/turbin-type. Beregnes alltid ved BEP ($Q^*$, $H^*$), $\omega$ i rad/s:

> $N_{sp} = \frac{\omega \sqrt{Q^*}}{(gH^*)^{3/4}}$

| $N_{sp}$ | Type |
|---|---|
| $< 1{,}5$ | Sentrifugal (radial) |
| $1{,}5 – 3{,}5$ | Mixed-flow |
| $> 3{,}5$ | Aksial |

---

## Pelton-turbin (impuls)

Brukes ved **høyt fall, lav flow**. All energi omdannes til kinetisk energi i dysen før skovlene.

**Strålehastighet** ($C_v \leq 1$ er tapsfaktor):

> $V_j = C_v\sqrt{2gH_{gross}}$

**Stråle-diameter:**

> $D_j = \sqrt{\frac{4Q}{\pi V_j}}$

**Optimal periferihastighet** (maks effekt):

> $U_{opt} = r\omega_{opt} = \frac{V_j}{2} \quad \Rightarrow \quad \omega_{opt} = \frac{V_j}{2r}$

**Ideell maksimal akseltilført effekt:**

> $\dot{W}_{aksel,ideell,max} = \frac{\rho Q V_j^2}{4}(1 - \cos\beta)$

der $\beta$ = skovlvinkel (typisk $\beta \approx 165°$)

**Virkningsgrad:**

> $\eta_{turbin} = \frac{\text{bhp}}{\dot{W}_{aksel,ideell,max}}$

---

## Nøkkelbegreper og omregning

| Symbol | Størrelse | Enhet |
|---|---|---|
| $Q$ | Volumstrøm | $m^3/s$ |
| $H$ | Netto pumpehøyde | m |
| $\omega$ | Vinkelhastighet | rad/s ($= \text{rpm} \cdot 2\pi/60$) |
| bhp | Akseltilført effekt | W |
| $\eta$ | Virkningsgrad | – |
| $P_v$ | Damptrykk | Pa |
| $C_v$ | Hastighetstapskoeffisient (dyse) | – |

| Fra | Til | Faktor |
|---|---|---|
| bhp | W | $\times\ 745{,}7$ |
| gpm | m³/s | $\times\ 0{,}000063$ |
| gpm | L/s | $\times\ 0{,}063$ |
| ft | m | $\times\ 0{,}305$ |
| inch | cm | $\times\ 2{,}54$ |
