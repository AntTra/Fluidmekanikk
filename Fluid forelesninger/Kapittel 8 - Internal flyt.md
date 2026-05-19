# Kapittel 8 – Intern strøm

## Innledning og strømningsregimer

**Intern strøm** – fluid omsluttet av vegger (rør, kanal).

Regimene bestemmes av Reynolds-tall ($D$ = rørdiameter):

> $Re = \frac{\rho V D}{\mu} = \frac{VD}{\nu}$

| Re | Regime |
|---|---|
| $< 2300$ | Laminær |
| $2300 – 4000$ | Overgangsone |
| $> 4000$ | Turbulent |

---

## Fullt utviklet strøm

**Inngangslengde** – strekningen fra innløpet til hastighetsprofilen er stabil:
- Laminær: $L_h \approx 0{,}06 \, Re \cdot D$
- Turbulent: $L_h \approx 4{,}4 \, Re^{1/6} \cdot D$

### Laminær hastighetsprofil (Hagen-Poiseuille)

Parabolsk profil:

> $u(r) = U_{max}\left(1 - \frac{r^2}{R^2}\right), \qquad U_{max} = 2V$

der $V = Q/A$ er gjennomsnittshastigheten.

Friksjonsfaktor for laminær strøm:

> $f = \frac{64}{Re}$

### Turbulent hastighetsprofil

Flatere profil, $\alpha \approx 1$ (god tilnærming).

---

## Darcy-Weisbach (major tap)

Trykkfall / tapshøyde langs et rør med lengde $L$:

> $h_f = f \frac{L}{D} \frac{V^2}{2g}$

> $\Delta P = f \frac{L}{D} \frac{\rho V^2}{2}$

- $f$ – Darcy friksjonsfaktor (dimensjonsløs)
- $D$ – indre rørdiameter \[m\]
- $V$ – gjennomsnittshastighet \[m/s\]

---

## Friksjonsfaktoren $f$ – Moody-diagram og Colebrook

For **turbulent strøm** i rør med relativ ruhet $\varepsilon/D$:

**Colebrook-likningen** (implisitt i $f$):

> $\frac{1}{\sqrt{f}} = -2{,}0 \log\left(\frac{\varepsilon/D}{3{,}7} + \frac{2{,}51}{Re\sqrt{f}}\right)$

Løses iterativt eller leses av **Moody-diagrammet** ($Re$ på x-aksen, $\varepsilon/D$ som parameter).

**Typiske ruhetverdier:**

| Material | $\varepsilon$ \[mm\] |
|---|---|
| Glass / plast | $\approx 0$ |
| Kommersielt stål | $0{,}046$ |
| Galvanisert jern | $0{,}15$ |
| Støpejern | $0{,}26$ |
| Betong | $0{,}3 – 3$ |

---

## Minor tap (lokale tap)

Tap ved innsnevringer, utvidelser, ventiler, bøyer, etc.:

> $h_m = K_L \frac{V^2}{2g}$

**Typiske $K_L$-verdier:**

| Komponent | $K_L$ |
|---|---|
| Skarp innløp | $0{,}5$ |
| Utløp (til reservoar) | $1{,}05$ |
| 90° bøy (standard) | $0{,}3 – 0{,}9$ |
| Fullt åpen kulventil | $\approx 0{,}2$ |
| Delvis lukket ventil | $\gg 1$ |

---

## Total tapshøyde

> $h_{L,total} = h_{f} + \sum h_m = f\frac{L}{D}\frac{V^2}{2g} + \sum K_L \frac{V^2}{2g} = \left(f\frac{L}{D} + \sum K_L\right)\frac{V^2}{2g}$

---

## Energilikningen for rørsystem

Sett inn i utvidet Bernoulli (fra Kap 5):

> $\frac{P_1}{\rho g} + \frac{V_1^2}{2g} + z_1 + h_{pumpe} = \frac{P_2}{\rho g} + \frac{V_2^2}{2g} + z_2 + h_L$

**Nødvendig pumpehøyde:**

> $H_{nødvendig} = (z_2 - z_1) + \frac{P_2 - P_1}{\rho g} + \frac{V_2^2 - V_1^2}{2g} + h_L$

For åpne reservoarer ($P_1 = P_2 = P_{atm}$, $V_1 \approx V_2 \approx 0$):

> $H_{nødvendig} = (z_2 - z_1) + h_L$

---

## Fremgangsmåte for rørsystemoppgaver

1. Finn $Re$ → avgjør regime (laminær / turbulent)
2. Finn $\varepsilon/D$ → les $f$ fra Moody-diagram (eller bruk Colebrook)
3. Beregn $h_L = \left(f\frac{L}{D} + \sum K_L\right)\frac{V^2}{2g}$
4. Sett inn i energiligningen
5. Finn $Q = VA$ der $A = \pi D^2/4$
