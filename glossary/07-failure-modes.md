# 7. Failure modes

## Cavitation

| PT | EN | ES |
|----|----|-----|
| Cavitação | Cavitation | Cavitación |

(Defined in [§1 Hydraulics](./01-hydraulics.md). Listed here for
cross-reference.)

Vapor-bubble formation and collapse in low-pressure regions. Symptoms:
gravelly noise, vibration, head and efficiency loss, rapid impeller wear.
Cause: NPSHa < NPSHr, often due to clogged suction strainer, fluid
temperature rise, or process upset that exceeds suction-side capacity.

**Distinguishing cavitation from other failures**: cavitation noise is
random in frequency and "shotty"; bearing failure noise is more
deterministic, increasing with rotation rate.

---

## Recirculation

| PT | EN | ES |
|----|----|-----|
| Recirculação interna | Internal recirculation | Recirculación interna |

Damaging flow reversal inside the impeller when operating well below BEP
(typically < 50% BEP). Liquid that should flow outward through the
impeller channels instead recirculates back, generating shear, vortex
shedding, and impact loads on the impeller.

**Distinguishing recirculation from cavitation**: both produce noise, but
recirculation noise is steady (single tone), while cavitation noise is
random. Recirculation occurs at low flow; cavitation can occur at any
flow if suction conditions are inadequate.

**Mitigation**: do not operate centrifugal pumps continuously below 70%
BEP. For variable-flow services that must drop below 50% BEP, install a
**bypass loop** to recirculate flow back to suction tank when process
demand is low.

---

## Dry running

| PT | EN | ES |
|----|----|-----|
| Operação a seco | Dry running | Funcionamiento en seco |

Pump operating without fluid in the casing. For mechanical seals, dry
running burns the faces in seconds because there is no fluid film for
heat dissipation. For positive-displacement pumps, dry running causes
gear-on-casing or rotor-on-casing metal-to-metal contact within the same
timescale.

**Mitigation**:

- **Level interlocks** on suction tanks
- **Flow switches** that detect zero flow
- **Pressure switches** on discharge that trigger shutdown if no
  pressure builds up
- For mechanical seals: dual-seal arrangements with pressurized barrier
  fluid

---

## Water hammer

| PT | EN | ES |
|----|----|-----|
| Golpe de aríete | Water hammer | Golpe de ariete |

Pressure wave caused by sudden flow change (valve closure, pump trip).
Pressure spike can reach **5-10× normal operating pressure** and damage
piping, casings, and check valves.

**Joukowsky's equation** estimates the peak:

```
ΔP = ρ × c × Δv

Where:
  ρ = fluid density (kg/m³)
  c = wave celerity in fluid + pipe (≈ 1.000-1.300 m/s for water in steel pipe)
  Δv = velocity change (m/s)
```

For a 3 m/s flow stop in water-in-steel pipe, ΔP ≈ 30-40 bar — far above
typical pump rated pressures.

**Mitigation**:

- **Slow-closing valves** (motorized actuators with 30-60 s ramp)
- **Surge tanks / accumulators** at vulnerable points
- **Pressure-relief valves** sized for the surge volume
- **Pump soft-stop** sequences (controller ramps speed down rather than
  tripping)

---

## Misalignment

| PT | EN | ES |
|----|----|-----|
| Desalinhamento | Misalignment | Desalineación |

Coupling-to-driver concentricity error. Two flavors:

- **Parallel misalignment**: shaft centerlines offset (TIR > 0.05 mm)
- **Angular misalignment**: shaft centerlines at an angle (> 0.05 mm/100 mm coupling diameter)

Both transmit cyclic loads to bearings, accelerating wear. Vibration
spectrum shows a strong **2× rotation** peak.

**Cold versus hot alignment**: thermal growth shifts the alignment after
the pump warms up. For hot pumps (thermal-oil at 250 °C), the cold-
alignment must be deliberately offset so that hot operation lands within
tolerance. The offset is supplier-specific; pull from the IOM manual.

---

## Imbalance

| PT | EN | ES |
|----|----|-----|
| Desbalanceamento (impeller) | Imbalance | Desequilibrio |

Mass imbalance in the rotating assembly. Causes vibration peak at **1×
rotation** in the spectrum.

Causes: impeller damage (broken vane, erosion), accumulated deposits on
impeller, manufacturing defect, replacement impeller not field-balanced.

**Mitigation**: dynamic balance per ISO 21940-11 (formerly ISO 1940-1).
Field balance kits exist for pumps that cannot be sent to a balance shop.

---

## Bearing failure

| PT | EN | ES |
|----|----|-----|
| Falha de mancal / rolamento | Bearing failure | Fallo de cojinete |

Most common pump-component failure. Causes:

- **Improper lubrication**: too much grease causes overheating; too little causes wear; wrong type causes incompatibility
- **Contamination**: water ingress through the breather, particulates from process side
- **Misalignment**: external loading exceeds bearing capacity
- **Overspeed**: bearing exceeds maximum design rpm
- **Electrical erosion** (PT: erosão elétrica; ES: erosión eléctrica): VFD-induced shaft currents pit the bearing races. Mitigated by insulated bearings on the non-drive end OR shaft grounding rings.

---

## Seal failure

| PT | EN | ES |
|----|----|-----|
| Falha de selo / vedação | Seal failure | Fallo de sello |

Mechanical seal failure modes:

- **Face wear** (normal): typical 2-5 year life depending on duty
- **Thermal shock**: rapid temperature change cracks the face
- **Crystallization**: fluid solidifies between faces, plucks face material
- **Cavitation behind face**: vapor pockets erode face seating
- **Dry running** (see above)
- **Chemical attack**: incompatible seal-face or O-ring material

Diagnosis: dismantle and inspect faces. Wear pattern tells the story —
even circumferential wear is normal; fracture indicates thermal shock;
crystalline deposits indicate fluid issue; pitted faces indicate
cavitation or vapor lock.

---

## Erosion

| PT | EN | ES |
|----|----|-----|
| Erosão | Erosion | Erosión |

Material loss from impingement of solid particles or high-velocity fluid
on impeller, casing, or wear rings. Common in:

- Slurry duty
- Seawater with sand
- Pulp & paper white-water
- High-pressure deluge or fire-water service

Mitigation: hardened materials (CD4MCu, ceramic-coated wear rings),
oversize pump for lower velocities, replace impellers on inspection
schedule.

---

## See also

- [Hydraulic fundamentals](./01-hydraulics.md) — for cavitation theory
- [Mechanical seals](./03-seals.md) — for seal-failure mitigation
- [Materials](./04-materials.md) — for erosion-resistance choices
- [pump-engineering-handbook §1.2 (selection)](https://github.com/fb-bombas/pump-engineering-handbook/tree/main/docs/01-centrifugal)
