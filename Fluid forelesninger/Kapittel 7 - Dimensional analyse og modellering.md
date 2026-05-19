# Kapittel 7 – Dimensjonsanalyse og modellering

## Buckingham Pi-teorem

Hvis et problem har $n$ variabler og $k$ grunnleggende dimensjoner (M, L, T, Θ), så kan det beskrives av:

> $n - k$ dimensjonsløse $\Pi$-grupper

**Fremgangsmåte:**
1. List alle $n$ relevante variabler
2. Finn $k$ = antall uavhengige dimensjoner
3. Velg $k$ repeterende variabler (må ikke danne en $\Pi$ seg imellom)
4. Kombiner hver gjenværende variabel med de repeterende for å danne $\Pi$-grupper
5. Sjekk at alle $\Pi$ er dimensjonsløse

---

## Viktige dimensjonsløse tall

| Tall | Definisjon | Fysisk tolkning |
|---|---|---|
| Reynolds | $Re = \frac{\rho V L}{\mu} = \frac{VL}{\nu}$ | Treghets- / viskøse krefter |
| Froude | $Fr = \frac{V}{\sqrt{gL}}$ | Treghets- / gravitasjonskrefter |
| Mach | $Ma = \frac{V}{c}$ | Treghets- / kompressibilitetskrefter |
| Weber | $We = \frac{\rho V^2 L}{\sigma}$ | Treghets- / overflatespenningskrefter |
| Euler | $Eu = \frac{\Delta P}{\rho V^2}$ | Trykk- / treghetskreftter |

---

## Dynamisk likhet og modellering

For at modell og prototype skal oppføre seg likt, kreves **dynamisk likhet**:
- Geometrisk likhet (samme form, skala $\lambda = L_m/L_p$)
- Kinematisk likhet (samme hastighetsprofil-form)
- Dynamisk likhet (samme relevante $\Pi$-grupper)

**Eksempel – rørstrøm:**  
Krev $Re_m = Re_p$:

> $\frac{V_m L_m}{\nu_m} = \frac{V_p L_p}{\nu_p} \quad \Rightarrow \quad V_m = V_p \frac{L_p}{L_m} \frac{\nu_m}{\nu_p}$

**Kraftskalering:**

> $\frac{F_m}{F_p} = \frac{\rho_m V_m^2 L_m^2}{\rho_p V_p^2 L_p^2}$

---

## Moody-formelen (effektivitetsskalering, Kap 14)

Et spesialtilfelle av modelllikhet for pumper:

> $\eta_{B} = 1 - (1 - \eta_{A})\left(\frac{D_A}{D_B}\right)^{1/5}$
