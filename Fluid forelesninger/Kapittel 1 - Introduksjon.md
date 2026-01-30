>Fluid statikk - Newtons 1. lov
>Fluid kinematikk - kinematisk beskrivelse
>Fluid dynamikk - Newtons 2. lov

Forskjellen på kinematikk og dynamikk vil være henholdsvis være geometrien/hastigheten vs kraften som påføres et element

# Grunnleggende begreper:
**Vegg - betingelser:** Lag en normalvektor fra veggen som er 0 for hastighet. Dette avhenger ut i fra hvilken retning vektoren har, men for en vegg så er denne hastigheten alltid 0.

**Heft - betingelse: "No-slip".** Treghet i fluid ved vegg. Ingen hastighet langs veggen altså. Dette skyldes på grunn av viskositet/seighet/klissete

>**Dynamisk viskositet $\mu$ vs kinematisk viskositet $\nu$**: De har ulike enheter (se enhetslista). Deler man Dynamisk på kinematisk så får man tetthet $\rho$. De pleier å være ganske små

>$\rho_{vann}\approx 1000$
>$\rho_{luft}\approx 1.24 kg/m^{-3}$

Hastighet v = ui+vj+wk. Left side is cartesian. Bruker man hastighet i kartesisk rom så vil hastigheten tilhøre et bestemt rom i verdenen og ikke partikkelen. 

**U** er ofte en notasjon for vektoren parallelt med veggen. 

Jukser man så kan man si at det ikke er friksjon langs veggen, så da vil jo hastigheten være gjennomsnitt og ikke variere som en kurve fra veggen. 

Dette er jo ikke sånn i virkeligheten. Dersom man har festet en fluid til seafloor så har den lyst til å bli

**Couette strøminng** - Lineært hastighetsprofil $u = V * u/h$. Hastigheten fra en vegg til en annen i f.ek.s en tube er lineært(en rett strek). Det som er morsomt med dette problemet er at den ene veggen beveger seg mens den andre står stille. Dette beskriver hvorfor hastighetsprofilen er lineær

> Newtons friksjonslov
> Dersom man ikke regner med friksjon så vil man kunne si at man kan regne med at det er hastighet langs veggen

Hvis dynamisk viskositet er 0 så bare glir fluidet. Flat hastighetsprofil
Man kan utnytte romderiverte for å stryke ut variabler når de ikke endrer seg. 
# Klassifisering av strømming

> Viskøs vs ikke viskøs
> Intern strømning (tube) vs ekstern (rundt et legeme)
> Kompressibel vs inkompressibel. $\rho$ er konstant i sistnevnte. Dette er ikke riktig i virkeligheten, men er riktig i dette faget da tettheten varierer lite.
>For gass, sjekk mach-tall. Dersom Ma<0.3 så regner vi inkompressibelt. Ma = local flow/lydhastighet
>Laminær vs turbulent. Viskøse krefter -> laminært. Inertialkrefter -> turbulent
> Stasjonært vs ikke-stasjonært. Finn rett laminære strømninger vs harmoniske virvler men fortsatt laminært

Inertial/Viskøse krefter = $m(dU/dt) /\tau A \sim \rho*L*U/\mu = Re = LU/V$
