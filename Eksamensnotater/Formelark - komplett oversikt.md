# Formelark – komplett oversikt med bruksområder

---

## Materialegenskaper

### Ideell gasslov (2-4)
> $P = \rho R T, \qquad R_{luft} = 287\ \text{Pa·m}^3/\text{kg·K}$

**Bruk:** Finn tetthet til gass når trykk og temperatur er kjent. $T$ må være i Kelvin. Ikke bruk for væske ($\rho \approx \text{konst}$ for væske).

### Kinematisk viskositet
> $\nu = \frac{\mu}{\rho}$

**Bruk:** Omregning mellom dynamisk ($\mu$) og kinematisk ($\nu$) viskositet. Trengs for Re-tall.

### Skjærspenning (2-33)
> $\tau_{xy} = \mu\!\left(\frac{\partial u}{\partial y} + \frac{\partial v}{\partial x}\right)$

**Bruk:** Finn skjærspenning i fluid (f.eks. på vegg). Forenkles til $\tau = \mu\, du/dy$ for enkel 1D strøm (Couette). Veggkraft = $\tau \cdot A$.

### Overflatespenning – såpeboble (2-41)
> $\Delta P = \frac{4\sigma_s}{R}$

**Bruk:** Trykkdifferanse inne i en boble (faktor 4 for to flater). For én flate (dråpe): $\Delta P = 2\sigma_s/R$.

---

## Trykk og hydrostatikk (Kap 3)

### Hydrostatisk trykkfordeling (3-9)
> $\frac{dP}{dz} = -\rho g$

**Bruk:** Trykk i stillestående fluid. Integrert: $P_2 = P_1 + \rho g (z_1 - z_2)$. Grunnlag for manometre og dybdetrykk. $z$ positiv oppover.

### Kraft på neddykket plan flate (3-19)
> $F_R = (P_0 + \rho g h_C)\,A = P_C\,A$

**Bruk:** Total kraft på en flat, neddykket flate (luke, plate, dam). $h_C$ = dybde til flatens tyngdepunkt. $P_0$ = overflatetrykk.

### Trykksenter (3-22a,b)
> $y_P = y_C + \frac{I_{xx,C}}{[y_C + P_0/(\rho g \sin\theta)]\,A}$

For $P_0 = 0$ (manometrisk):
> $y_P = y_C + \frac{I_{xx,C}}{y_C A}$

**Bruk:** Finner hvor resultantkraften angriper (alltid under tyngdepunktet). $I_{xx,C}$ = annet arealmoment om senteraksen (rektangel: $bh^3/12$, sirkel: $\pi R^4/4$).

### Trykk i rigid-legeme-bevegelse
> $\vec{\nabla}P = \rho\,\vec{g}_{eff}$

der:
> $\vec{g}_{eff} = \vec{g} - \vec{a} \quad$ (lineær akselerasjon)
> $\vec{g}_{eff} = \vec{g} + \omega^2 r\,\vec{e}_r \quad$ (rotasjon)

**Bruk:** Fluid som akselererer eller roterer som ett stivt legeme (ingen intern strøm). Sentrifuge: $dP/dr = \rho\omega^2 r$. Hvis $\omega^2r/g \gg 1$: dropp $\vec{g}$.

---

## Kinematikk (Kap 4)

### Materiell derivert / akselerasjon (4-9, 4-11)
> $\frac{D\vec{V}}{Dt} = \frac{\partial\vec{V}}{\partial t} + (\vec{V}\cdot\nabla)\vec{V}$

**Bruk:** Akselerasjon til en fluidpartikkel (Lagrangiansk) uttrykt ved Eulerianske felt. Trengs i N-S-utledning. I stasjonær strøm faller $\partial/\partial t$ bort.

### Langs en strømlinje (4-15)
> $\frac{dr}{V} = \frac{dx}{u} = \frac{dy}{v} = \frac{dz}{w}$

**Bruk:** Finn strømlinjenes form analytisk. Løs som ODE: $dy/dx = v/u$.

### Vorticitet (4-28,29)
> $\vec{\zeta} = 2\vec{\Omega} = \vec{\nabla}\times\vec{V}$

**Bruk:** Mål på rotasjon i fluidet. Irrotasjonell strøm: $\vec{\zeta} = 0$.

### Reynolds transport theorem (4-41)
> $\frac{dB_{sys}}{dt} = \frac{d}{dt}\!\int_{KV}\!\rho b\,dV + \oint_{KF}\rho b\,(\vec{V}_r\cdot\hat{n})\,dA$

**Bruk:** Kobling mellom system (Lagrangiansk) og kontrollvolum (Euleriansk). Grunnlag for alle KV-ligninger (masse, moment, energi). Sjelden direkte brukt på eksamen – men grunnlaget for neste seksjon.

---

## Masse, Bernoulli og energi (Kap 5)

### Volumstrøm (5-8)
> $Q = \dot{V} = \int_{A_c} \vec{V}_r\cdot\hat{n}\,dA$

**Bruk:** Forenklet til $Q = VA$ (uniform hastighet) eller $Q = V_{avg}A$. Brukes overalt.

### Massebalanse (5-17)
> $\frac{d}{dt}\!\int_{KV}\!\rho\,dV + \oint_{KF}\rho(\vec{V}_r\cdot\hat{n})\,dA = 0$

Stasjonær inkompressibel:
> $\sum V_{ut}A_{ut} = \sum V_{inn}A_{inn}$

**Bruk:** Første steg i nesten alle oppgaver. Finn ukjent hastighet.

### Bernoulli – ustasjonær kompressibel (5-44)
> $\int\frac{dP}{\rho} + \int\frac{\partial V}{\partial t}\,ds + \frac{V^2}{2} + gz = \text{konst}$

**Bruk:** Sjelden brukt direkte — den generelle formen. Brukes kun ved kompressibel eller ustasjonær strøm.

### Bernoulli – stasjonær inkompressibel (5-48)
> $\frac{P}{\rho g} + \frac{V^2}{2g} + z = \text{konst}$

**Bruk:** Enkel, friksjonsfri strøm langs én strømlinje. Dyser, fri-stråler, Pitot-rør. **Ikke bruk** hvis det er friksjon, pumpe eller turbin.

### Energilikning – generell (5-60)
> $\dot{Q}_{inn} + \dot{W}_{aksel,inn} = \frac{d}{dt}\!\int_{KV}\!e\rho\,dV + \oint_{KF}\!\left(\frac{P}{\rho}+e\right)\rho(\vec{V}_r\cdot\hat{n})\,dA$

der $e = u + V^2/2 + gz$

**Bruk:** Fullstendig termodynamisk energibalanse. Grunnlaget for 5-77.

### Energilikning – ett innløp/utløp stasjonær (5-77)
> $\frac{P_1}{\rho g} + \alpha_1\frac{V_1^2}{2g} + z_1 + h_{pumpe} = \frac{P_2}{\rho g} + \alpha_2\frac{V_2^2}{2g} + z_2 + h_{turbin} + h_L$

**Bruk:** Standardformel for alle rørsystem-oppgaver. Kombiner med Darcy-Weisbach for $h_L$.

Vanlige forenklinger:

| Situasjon | Forenkl |
|---|---|
| Stort reservoar | $V \approx 0$ ved overflaten |
| Åpen overflate | $P = P_{atm}$ (kansellerer) |
| Turbulent rør | $\alpha = 1{,}05 \approx 1$ |
| Laminær rør | $\alpha = 2$ |

### Kinetisk energikorreksjonsfaktor
> $\alpha \approx 2$ (laminær), $\quad \alpha \approx 1{,}05$ (turbulent)

**Bruk:** Korrigerer for at hastighetsprofilen ikke er flat. Sett ofte $\alpha = 1$ (oppgitt i oppgave).

---

## Momentum (Kap 6)

### Lineær momentumlikning (6-16)
> $\sum\vec{F} = \frac{d}{dt}\!\int_{KV}\!\rho\vec{V}\,dV + \oint_{KF}\rho\vec{V}(\vec{V}_r\cdot\hat{n})\,dA$

Stasjonær:
> $\sum\vec{F} = \sum_{ut}\dot{m}\vec{V} - \sum_{inn}\dot{m}\vec{V}$

**Bruk:** Finn kraft på rørbow, dyse, vane, brakkettfeste. Skill alltid i $x$- og $y$-komponent. $\sum\vec{F}$ inkluderer trykk, tyngde og veggkraft.

### Netto trykkraft på lukket KF
> $\vec{F}_{trykk} = -\oint_{KF} P_{gauge}\,\hat{n}\,dA$

**Bruk:** Beregn trykkbidrag på kontrollflaten i momentumligningen.

---

## Intern strøm (Kap 8)

### Kritisk Reynolds-tall
> $Re_{krit} \approx 2300$

**Bruk:** $Re < 2300$ → laminær. $Re > 4000$ → turbulent. Mellom: overgangsone.

### Inngangslengde (8-6,7)
> $\frac{L_{h,lam}}{D} \approx 0{,}05\,Re \qquad \frac{L_{h,turb}}{D} \approx 1{,}359\,Re^{1/4}$

**Bruk:** Sjekk om strømmen er fullt utviklet (brukes sjelden i oppgaver, men greit å kjenne til).

### Darcy friksjonsfaktor – laminær (8-23)
> $f = \frac{64}{Re}$

**Bruk:** Kun for laminær rørstøm ($Re < 2300$). Direkte formel, ingen diagram nødvendig.

### Rørtapshøyde (8-24)
> $h_L = f\frac{L}{D}\frac{V^2}{2g}$

**Bruk:** Major-tap i rør. Sett inn $f$ fra laminær-formel eller Colebrook/Moody.

### Colebrook (8-50)
> $\frac{1}{\sqrt{f}} = -2{,}0\log\!\left(\frac{\varepsilon/D}{3{,}7}+\frac{2{,}51}{Re\sqrt{f}}\right)$

**Bruk:** Turbulent strøm i ru rør. Implisitt — løses iterativt (start med $f \approx 0{,}02$, iterér 2–3 ganger).

### Haaland (8-51)
> $\frac{1}{\sqrt{f}} \simeq -1{,}8\log\!\left[\frac{6{,}9}{Re}+\left(\frac{\varepsilon/D}{3{,}7}\right)^{1{,}11}\right]$

**Bruk:** Eksplisitt alternativ til Colebrook. Raskere å bruke for hånd, nøyaktighet $\pm 2\%$.

### Total tapshøyde (8-58)
> $h_{L,total} = \sum f\frac{L}{D}\frac{V^2}{2g} + \sum K_L\frac{V^2}{2g}$

**Bruk:** Rørsystem med flere segmenter og fittings. Sett inn i energilikning (5-77).

---

## Differensialanalyse (Kap 9)

### Kontinuitetslikning – generell (9-5)
> $\frac{\partial\rho}{\partial t} + \vec{\nabla}\cdot(\rho\vec{V}) = 0$

### Inkompressibel kontinuitet (9-16)
> $\vec{\nabla}\cdot\vec{V} = 0$

**Bruk:** Sjekk om gitt hastighetsfelt er fysisk mulig. I Cartesisk: $\partial u/\partial x + \partial v/\partial y + \partial w/\partial z = 0$.

### Kontinuitet i sylinderkoodinater (9-12)
> $\frac{\partial\rho}{\partial t} + \frac{1}{r}\frac{\partial(r\rho u_r)}{\partial r} + \frac{1}{r}\frac{\partial(\rho u_\theta)}{\partial\theta} + \frac{\partial(\rho u_z)}{\partial z} = 0$

**Bruk:** Rørstøm, aksesymmetriske problemer. For inkompressibel: $\rho = \text{konst}$.

### Strømfunksjon $\psi$ (9-20,27,29)
Cartesisk: $u = \partial\psi/\partial y,\quad v = -\partial\psi/\partial x$  
Sylinder: $u_r = \frac{1}{r}\partial\psi/\partial\theta,\quad u_\theta = -\partial\psi/\partial r$

**Bruk:** $\psi = \text{konst}$ langs strømlinje. Automatisk tilfredsstiller kontinuitet.

### Navier-Stokes – inkompressibel (9-60)
> $\rho\frac{\partial\vec{V}}{\partial t} + \rho(\vec{V}\cdot\nabla)\vec{V} = -\nabla P + \rho\vec{g} + \mu\nabla^2\vec{V}$

**Bruk:** Finn hastighetsprofil og trykkfordeling analytisk. Forenkl ledd for ledd:

| Antagelse | Ledd = 0 |
|---|---|
| Stasjonær | $\partial\vec{V}/\partial t$ |
| Fullt utviklet / uniform | $(\vec{V}\cdot\nabla)\vec{V}$ |
| 1D strøm | alt unntatt én komponent |

Resulterer i ODE → integrer to ganger → bruk randbetingelser (no-slip: $u=0$ ved vegg).

**Standardresultater:**
- Couette (plater, ingen $\nabla P$): $u = U\,y/h$ — lineært
- Poiseuille (rør): $u_z = \frac{1}{4\mu}(-dP/dz)(R^2-r^2)$ — parabolsk, $U_{max} = 2V$

### N-S i sylinderkoodinater (vedlegg 1)

$r$-komponent (forenklet for fullt utviklet aksial strøm):
> $0 = -\frac{\partial P}{\partial z} + \mu\frac{1}{r}\frac{d}{dr}\!\left(r\frac{du_z}{dr}\right)$

**Bruk:** Hagen-Poiseuille-strøm i rør. Integrer to ganger, bruk $u_z(R)=0$ og symmetri.

---

## Ekstern strøm (Kap 10–11)

### 2D irrotasjonell strøm (10-28,30)
> $\nabla^2\psi = 0$

**Bruk:** Potentialstrøm. Ikke i pensum.

### Grenselagtykkelse – flat plate (Tabell 10-4)
> $\frac{\delta}{x} \approx \frac{4{,}91}{Re_x^{1/2}}$ (laminær), $\quad \frac{\delta}{x} \approx \frac{0{,}16}{Re_x^{1/7}}$ (turbulent)

**Bruk:** Finn grenselagtykkelse langs plate. $Re_x = Vx/\nu$ (lokal Re).

### Lokal hudfrisksjonskoeffisient (10-98)
> $C_{f,x} = \frac{\tau_w(x)}{\frac{1}{2}\rho U^2}$

**Bruk:** Dimensjonsløs lokal veggskjærspenning. Integrer over flaten for total friksjonskraft.

### Drag og løft (11-5,6)
> $C_D = \frac{F_D}{\frac{1}{2}\rho V^2 A}, \qquad C_L = \frac{F_L}{\frac{1}{2}\rho V^2 A}$

**Bruk:** Finn kraft fra koeffisient (lest av diagram eller tabell). $A$ = frontalareal for drag, planformareal for løft.

---

## Vedlegg 1 – Sylinderkoodinater (sammendrag)

Alle N-S-komponenter i sylinderkoodinater er på vedlegget. Fremgangsmåte:

1. Identifiser hvilke hastighetskomponer som er null ($u_r$, $u_\theta$, $u_z$)
2. Stryk ledd som inneholder disse
3. Sjekk stasjonær ($\partial/\partial t = 0$) og symmetri ($\partial/\partial\theta = 0$)
4. Løs gjenværende ODE

**Typisk for rørstøm:** kun $u_z(r)$ gjenværende → Hagen-Poiseuille.  
**Typisk for roterende strøm:** kun $u_\theta(r)$ → Taylor-Couette.
