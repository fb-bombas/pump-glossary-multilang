# 3. Mechanical seals and shaft sealing

## Mechanical seal

| PT | EN | ES |
|----|----|-----|
| Vedação mecânica / Selo mecânico | Mechanical seal | Sello mecánico |

A precision dynamic seal between a rotating shaft and a stationary
casing, consisting of:

- A **rotating face** (mounted on the shaft, often silicon carbide or carbon)
- A **stationary face** (mounted in the casing, typically silicon carbide or tungsten carbide)
- **Spring loading** to maintain face contact
- **Secondary seals** (O-rings, bellows) to seal against the shaft and casing

**Gotcha:** ABNT NBR 13929 prefers **"vedação mecânica"**; vendor catalogs
in Brazil more often use **"selo mecânico"**. Both are understood; in a
formal contract, follow the standard or pick one and be consistent. ES
practice strongly prefers "sello mecánico".

---

## Single mechanical seal

| PT | EN | ES |
|----|----|-----|
| Selo mecânico simples | Single mechanical seal | Sello mecánico simple / sencillo |

One pair of seal faces. Adequate for benign fluids at moderate temperature
and pressure. Fluid-side face is exposed to process fluid; the back side
is open to atmosphere.

---

## Double mechanical seal (dual seal)

| PT | EN | ES |
|----|----|-----|
| Selo mecânico duplo / Vedação dupla | Double mechanical seal / Dual seal | Sello mecánico doble |

Two pairs of seal faces in series, separated by a barrier or buffer
fluid. Used when:

- Process fluid is hazardous, toxic, flammable, or otherwise must not leak
- Process fluid is a poor lubricant (low viscosity, dirty, or shear-sensitive)
- Vapor-pressure considerations require positive face cooling

**Configurations** per API 682:

- **Arrangement 2** (PT: Arranjo 2; ES: Disposición 2): Two seals with **buffer fluid** at lower pressure than process — leakage flows inward to be safely vented
- **Arrangement 3** (PT: Arranjo 3; ES: Disposición 3): Two seals with **barrier fluid** at higher pressure than process — barrier fluid leaks slowly into process; no process leak to atmosphere

API 682 plan numbers (e.g., Plan 53A, Plan 54) describe the support-system
piping; the seal arrangement is separate.

---

## Packing (gland packing)

| PT | EN | ES |
|----|----|-----|
| Gaxeta / Empanque | Packing / Gland packing | Empaquetadura |

Older shaft-sealing technology: rings of compressible material (graphite
fibers, PTFE-impregnated yarns) packed into a stuffing box around the
shaft and compressed by a follower (the gland).

**Gotcha:** packing requires **continuous slow leakage** to lubricate
the shaft surface and dissipate friction heat (typical 30-60 drops per
minute). A "dry" packing is overcompressed and will burn out. Many
inexperienced operators tighten until leakage stops — the next failure
is shaft-sleeve scoring within hours.

Packing is largely obsolete for new industrial pumps but remains
appropriate for:

- Slurry / abrasive duty where mechanical seals fail rapidly
- Service where periodic re-tightening is acceptable
- Equipment retrofitted with packing-style stuffing boxes

PT term "empanque" appears occasionally and is acceptable; "gaxeta" is
standard. ES "empaquetadura" is uniformly used across Latin America.

---

## API 682 plan numbers

| Plan | Function | Common use |
|------|----------|-----------|
| Plan 11 | Recirculation from discharge to seal | Standard for clean fluids |
| Plan 13 | Recirculation from seal back to suction | High-pressure pumps where Plan 11 over-pressurizes seal |
| Plan 21 | External flush from clean source through cooler | Hot fluids requiring seal cooling |
| Plan 23 | Internal recirculation through cooler | Hot fluids where external flush adds dilution |
| Plan 32 | External flush, no return | Slurry / abrasive duty (seal flush dilutes process) |
| Plan 52 | Buffer-fluid system at low pressure (Arrangement 2) | Hazardous fluids with allowable inward leakage |
| Plan 53A | Pressurized barrier-fluid system (Arrangement 3) | Toxic fluids; barrier pressurized above process |
| Plan 54 | Externally pressurized barrier system | High-reliability barrier for critical service |

**Gotcha:** when bidding asks for "Plan 11", that is shorthand for
"single mechanical seal with recirculation from discharge". The seal
arrangement (single vs double) and the support-system plan are
**separate** specifications. Both must be in the RFQ.

---

## Stuffing box

| PT | EN | ES |
|----|----|-----|
| Caixa de gaxeta / Caixa de vedação | Stuffing box | Caja de empaquetadura |

The cavity around the shaft where the seal or packing sits. In modern
mechanical-seal pumps, the stuffing box is sized large enough to
accommodate cartridge seals; in older packing-style pumps, it is sized
for packing rings only.

**Big-bore stuffing box** (PT: caixa de vedação ampliada; ES: caja
ampliada): an oversized cavity that accommodates double mechanical seals
without modifying the casing. Now common in API 610 service.

---

## Cartridge seal

| PT | EN | ES |
|----|----|-----|
| Selo cartucho / Cartucho de vedação | Cartridge seal | Sello cartucho |

A pre-assembled mechanical seal supplied as a single unit on its own
sleeve. Eliminates field assembly (and field-assembly errors) — the
sleeve mounts on the shaft, the cartridge bolts to the stuffing-box
flange. Typical for modern API 682 installations.

**Why it matters:** cartridge seals reduce mean-time-between-failure
significantly because face installation and spring loading are factory-set.

---

## Seal flush

| PT | EN | ES |
|----|----|-----|
| Fluido de selagem / lavagem do selo | Seal flush | Fluido de sellado / Lavado del sello |

A clean fluid injected into the seal cavity to:

- Cool the seal faces
- Lubricate the running surfaces
- Flush away particulates that would damage faces
- Dilute corrosive species at the face

Flush sources include process fluid (Plan 11), external clean fluid
(Plan 32), or recirculated buffer fluid (Plan 52).

---

## See also

- [Pump types](./02-pump-types.md)
- [Failure modes](./07-failure-modes.md)
