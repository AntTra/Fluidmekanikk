# Kapittel 5 – Masse, Bernoulli og energilikninger

## Kontinuitetslikningen (massebalanse)

Generell form for kontrollvolum (fra RTT med $b = 1$):

> $\frac{d}{dt}\int_{KV} \rho \, dV + \int_{KF} \rho \, (\vec{V} \cdot \hat{n}) \, dA = 0$

For **stasjonær, inkompressibel** strøm (mest brukt):

> $\sum V_{ut} A_{ut} = \sum V_{inn} A_{inn}$

For ett innløp og ett utløp:

> $V_1 A_1 = V_2 A_2 = Q$

der $Q$ \[$m^3/s$\] er volumstrømmen.

**Massestrøm:** $\dot{m} = \rho Q = \rho V A$ \[kg/s\]

---

## Bernoulli-likningen

Gjelder langs en strømlinje, stasjonær, inkompressibel, **friksjonsfri** strøm:

> $\frac{P}{\rho g} + \frac{V^2}{2g} + z = \text{konst}$

Mellom to punkt:

> $\frac{P_1}{\rho g} + \frac{V_1^2}{2g} + z_1 = \frac{P_2}{\rho g} + \frac{V_2^2}{2g} + z_2$

**Energihøyder:**
- $P/\rho g$ — trykkshøyde
- $V^2/2g$ — hastighetshøyde
- $z$ — potensialhøyde
- Sum = total høyde (konstant langs strømlinje uten tap)

---

## Energilikningen (utvidet Bernoulli)

Inkluderer pumper, turbiner og tap — dette er den **mest brukte likningen på eksamen**:

> $\frac{P_1}{\rho g} + \frac{\alpha_1 V_1^2}{2g} + z_1 + h_{pumpe} = \frac{P_2}{\rho g} + \frac{\alpha_2 V_2^2}{2g} + z_2 + h_{turbin} + h_L$

- $h_{pumpe}$ — netto energihøyde tilført av pumpe \[m\]
- $h_{turbin}$ — netto energihøyde uttatt av turbin \[m\]
- $h_L$ — total tapshøyde (major + minor, se Kap 8) \[m\]
- $\alpha$ — kinetisk energikorreksjonsfaktor ($\alpha = 1$ for turbulent, $\alpha = 2$ for laminær — sett ofte $\alpha = 1$)

**Forenkling for store reservoarer:** $V \approx 0$ ved fri overflate

**Pumpehøyde fra effekt:**

> $h_{pumpe} = \frac{\dot{W}_{pumpe}}{\dot{m} g} = \frac{\dot{W}_{pumpe}}{\rho g Q}$

---

## Volumstrøm og gjennomsnittshastighet

> $Q = VA$ (uniform hastighet)

> $Q = \int_A u \, dA$ (varierende hastighetsprofil)

**Gjennomsnittshastighet** $V = Q/A$ brukes i energilikningen.

---

## Hydrostatisk trykk

For fluid i ro langs vertikal:

> $P_2 = P_1 + \rho g (z_1 - z_2)$

eller: $P = P_0 + \rho g h$ (der $h$ er dybde under referanse)
