# 1. Hydraulic fundamentals

## Flow rate

| PT | EN | ES |
|----|----|-----|
| Vazão (Q) | Flow rate (Q) | Caudal (Q) |

Volume of fluid moved per unit time. Industrial-pump units in PT and ES
contracts are typically **m³/h**; US specs use **gpm** (gallons per
minute). Conversion: 1 m³/h = 4,403 gpm.

**Gotcha:** "fluxo" in PT-BR informal usage sometimes substitutes for
"vazão" — incorrect. "Fluxo" is the qualitative concept of flow direction;
"vazão" is the quantitative rate.

In ES, **"flujo"** is the standard term in some technical contexts but
**"caudal"** is more precise for flow rate. ASME and API translations to
ES typically use "caudal".

---

## Total head

| PT | EN | ES |
|----|----|-----|
| Altura manométrica total (H) | Total head (H) | Altura manométrica total (H) |

Energy added to the fluid by the pump, expressed as height of fluid column.
For water at standard conditions, 10 m head ≈ 1 bar pressure. ABNT NBR
12515 prefers the term "altura manométrica"; "head" is widely understood
in PT industrial practice but is technically a loanword.

**Gotcha:** in Brazilian field practice, "cabeça" sometimes substitutes
for "altura manométrica". In a formal contract, use "altura manométrica
total" and define the unit (m of fluid column).

---

## Static head

| PT | EN | ES |
|----|----|-----|
| Altura manométrica estática | Static head | Altura manométrica estática |

The geometric difference in elevation between fluid surface at suction and
discharge, plus any pressure differential between source and destination
tanks. **Independent of flow rate.**

**Gotcha:** in some PT field manuals, "altura geométrica" appears as a
synonym. ABNT prefers "altura estática" because it includes the
pressure-differential contribution, not just geometric.

---

## Friction head / dynamic head

| PT | EN | ES |
|----|----|-----|
| Perda de carga / altura dinâmica | Friction head / dynamic head | Pérdida de carga / altura dinámica |

Head loss due to fluid friction in piping, fittings, valves, and process
equipment. Scales approximately with Q² for turbulent flow.

**Gotcha:** PT "perda de carga" maps to ES "pérdida de carga" cleanly,
but in EN "head loss" and "friction head" mean the same thing in most
contexts. Some EN texts reserve "head loss" for total dynamic losses
(friction + minor losses + acceleration head).

---

## Operating point

| PT | EN | ES |
|----|----|-----|
| Ponto de operação | Operating point | Punto de operación |

The intersection of the pump curve (H vs Q) and the system curve. Where
the pump actually runs.

**Gotcha:** in Spanish documents, **"punto de funcionamiento"** appears
as a synonym. Both are correct; "punto de operación" is closer to the
international convention.

---

## Best efficiency point (BEP)

| PT | EN | ES |
|----|----|-----|
| Ponto de melhor eficiência (PBE) | Best efficiency point (BEP) | Punto de máxima eficiencia (BEP) |

The flow rate at which the pump achieves its highest hydraulic efficiency.
On a centrifugal curve plot, BEP is where the η curve peaks.

**Gotcha:** the abbreviation "BEP" is universal in international practice;
PT engineers often write "PBE" as the formal abbreviation but verbal usage
is mostly "BEP" because it appears on imported curves and datasheets.

The **allowable operating region** per ANSI/HI 9.6.3 is **70%-110% of
BEP flow** for centrifugal pumps. Outside that band: recirculation
(below) or cavitation onset and motor overload (above).

---

## Net Positive Suction Head — Available (NPSHa)

| PT | EN | ES |
|----|----|-----|
| NPSH disponível / NPSHa | Net Positive Suction Head Available / NPSHa | NPSH disponible / NPSHa |

The absolute pressure available at the pump suction flange, expressed as
height of fluid column above vapor pressure.

```
NPSHa = (P_atm - P_vapor) / (ρ × g) - H_suction_static - H_suction_friction
```

Calculated by the buyer/system designer from system geometry, fluid
properties, and operating temperature. **Decreases** as fluid temperature
rises (vapor pressure increases) or as suction pipe friction grows.

**Gotcha:** "NPSH-d" appears in some Spanish documents as an abbreviation
for "disponible". The international convention is "NPSHa". Use NPSHa in
contracts to avoid ambiguity.

---

## Net Positive Suction Head — Required (NPSHr)

| PT | EN | ES |
|----|----|-----|
| NPSH requerida / NPSHr | Net Positive Suction Head Required / NPSHr | NPSH requerida / NPSHr |

The minimum NPSHa the pump needs to operate without cavitation, measured
per ANSI/HI 14.6 by the **3% drop method** — progressively reducing
suction pressure until pump head drops 3%.

NPSHr is **published by the manufacturer** and varies with flow rate; it
is not a single number but a curve.

**Gotcha:** "NPSHr" measured by 3% head drop is **not** the cavitation
inception point. Cavitation begins **before** 3% drop. ANSI/HI 9.6.1
recommends a margin (NPSHa - NPSHr) of at least 0.6 m, with 1.0 m
preferred for industrial duty.

---

## Cavitation

| PT | EN | ES |
|----|----|-----|
| Cavitação | Cavitation | Cavitación |

Formation of vapor bubbles in low-pressure regions of the impeller,
followed by violent collapse when pressure recovers. Damages metal,
generates noise, and degrades performance permanently.

Symptoms: irregular noise (often described as "gravel passing through the
pump"), vibration spikes, head and efficiency drop, rapid impeller wear.

**Gotcha:** in Spanish-to-English translation, "cavitación" sometimes
appears mistranslated as "caving in" or "collapse" — these are
mechanical-failure terms, not hydraulic-phenomenon terms.

---

## Affinity laws

| PT | EN | ES |
|----|----|-----|
| Leis de afinidade | Affinity laws | Leyes de afinidad |

Scaling relationships for centrifugal pumps under speed or impeller-
diameter changes (with the other held constant):

```
Speed change:        Q∝N    H∝N²    P∝N³
Diameter change:     Q∝D    H∝D²    P∝D³
```

**Gotcha:** the diameter law is exact only for small trims (< 10%).
Beyond that, hydraulic similarity breaks down and the curve must be
re-tested. This is a common source of off-design surprises after
impeller modifications.

---

## Specific speed

| PT | EN | ES |
|----|----|-----|
| Rotação específica (Ns) | Specific speed (Ns) | Velocidad específica (Ns) |

Dimensionless parameter characterizing impeller geometry:

```
Ns = N × √Q / H^(3/4)
```

(units vary by region — US, EU, and Brazilian conventions differ).

Used to classify impeller types: low Ns → radial flow (high head, low
flow); high Ns → axial flow (low head, high flow).

**Gotcha:** the numerical value of Ns differs by ~13% between US
customary and SI calculations because of unit conventions. Always state
the unit system when quoting Ns.

---

## See also

- [Pump types](./02-pump-types.md)
- [Failure modes](./07-failure-modes.md)
- [pump-engineering-handbook §1 (centrifugal pumps)](https://github.com/fb-bombas/pump-engineering-handbook/tree/main/docs/01-centrifugal)
