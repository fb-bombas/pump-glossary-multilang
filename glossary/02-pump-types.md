# 2. Pump types

## Centrifugal pump

| PT | EN | ES |
|----|----|-----|
| Bomba centrífuga | Centrifugal pump | Bomba centrífuga |

Rotodynamic pump using an impeller spinning inside a casing to add
kinetic energy to the fluid, then converting it to pressure energy
through a volute or diffuser. Most common pump type in industry.

**Variants:**

- **End-suction**: suction in line with shaft, discharge perpendicular
- **Split-case** (PT: bipartida; ES: bipartida): casing splits horizontally for maintenance
- **Multistage** (PT: multiestágio; ES: multietapa): multiple impellers in series for high head
- **Vertical inline** (PT: vertical em linha): suction and discharge on same horizontal line
- **Vertical turbine** (PT: turbina vertical; ES: turbina vertical): used for deep wells, sumps

---

## Normalized centrifugal pump

| PT | EN | ES |
|----|----|-----|
| Bomba centrífuga normalizada | Normalized centrifugal pump | Bomba centrífuga normalizada |

Centrifugal pump whose external dimensions follow ISO 2858 (international)
or ASME B73.1 (North America). Footprint, suction/discharge nozzles, and
shaft heights are standardized; hydraulic performance is not. Two
manufacturers' normalized pumps in the same size class will bolt onto the
same baseplate.

**Why this matters in procurement:** normalized geometry is cheaper to
maintain over a 15-year asset life because spare parts and even whole
pumps are interchangeable across vendors.

---

## Gear pump (positive displacement)

| PT | EN | ES |
|----|----|-----|
| Bomba de engrenagem | Gear pump | Bomba de engranajes |

Positive-displacement pump using two meshing gears that trap fluid in the
spaces between gear teeth and casing. Flow is approximately constant per
revolution regardless of discharge pressure (within rated envelope).

**Two main variants:**

- **External gear** (PT: engrenagem externa; ES: engranajes externos): two parallel shafts with gears meshing externally. Higher pulsation, simpler.
- **Internal gear** (PT: engrenagem interna; ES: engranajes internos): one driving gear with internal teeth meshing with a smaller idler gear. Lower pulsation, gentler on shear-sensitive fluids.

**Gotcha:** in Brazilian field practice, "bomba de engrenagens" (plural
"engrenagens") is also widespread — both are acceptable.

---

## Lobe pump

| PT | EN | ES |
|----|----|-----|
| Bomba de lóbulos | Lobe pump | Bomba de lóbulos |

Positive-displacement pump with two or three rotating lobes. Lobes do not
contact each other; they are timed by external gears. Common in food and
pharmaceutical applications because the gentle pumping action does not
shear sensitive fluids.

---

## Diaphragm pump

| PT | EN | ES |
|----|----|-----|
| Bomba de diafragma | Diaphragm pump | Bomba de diafragma |

Positive-displacement pump using a flexing diaphragm to push fluid
through check valves. Common variants: AODD (air-operated double
diaphragm), motorized diaphragm, and hydraulic diaphragm metering pumps.

**Gotcha:** AODD pumps are often spec'd for chemical and abrasive duty
but have lower volumetric efficiency than rotary pumps and consume
significantly more compressed-air energy per liter pumped.

---

## Axial flow pump

| PT | EN | ES |
|----|----|-----|
| Bomba axial / Bomba de fluxo axial | Axial flow pump | Bomba axial / Bomba de flujo axial |

Pump where fluid moves parallel to the shaft axis through a propeller-like
impeller. High flow, low head. Common in irrigation, drainage, large-
volume cooling water.

---

## Self-priming pump

| PT | EN | ES |
|----|----|-----|
| Bomba autoescorvante / autoaspirante | Self-priming pump | Bomba autoaspirante / autocebante |

Pump that can evacuate air from its suction line and start operating
without external priming. Most positive-displacement pumps are self-
priming; centrifugal pumps generally are not, with specialized
"self-priming centrifugal" variants the exception.

**Gotcha:** "autoescorvante" and "autoaspirante" are both used in PT-BR
field practice. ABNT standardized "autoaspirante". In ES, "autocebante"
is the term in Spain; "autoaspirante" and "auto-cebado" are common in
Latin America.

---

## Magnetic drive pump

| PT | EN | ES |
|----|----|-----|
| Bomba de acionamento magnético / sem selo | Magnetic drive pump / Sealless | Bomba de accionamiento magnético / sin sello |

Pump where the driver is coupled to the impeller through magnetic force
across a sealed containment shell — no shaft seal, no leakage path.
Used for hazardous, toxic, or expensive fluids where any leakage is
unacceptable.

**Gotcha:** "sem selo" (PT) and "sin sello" (ES) translate as "sealless",
which can be misleading because the pump still has a containment shell —
it just doesn't have a dynamic seal subject to wear.

---

## Submersible pump

| PT | EN | ES |
|----|----|-----|
| Bomba submersível | Submersible pump | Bomba sumergible |

Pump and motor designed to operate fully submerged in the fluid.
Common in deep wells, sewage, drainage, mining dewatering. Motor is
hermetically sealed; cooling is provided by the surrounding fluid.

---

## Sanitary pump

| PT | EN | ES |
|----|----|-----|
| Bomba sanitária | Sanitary pump / hygienic pump | Bomba sanitaria |

Pump certified for food, pharmaceutical, or biotech service per
3-A Sanitary Standards or EHEDG. Surfaces in contact with fluid are
polished to specified Ra, all dead spaces are eliminated, and the design
allows full Clean-In-Place (CIP) and Sterilize-In-Place (SIP) without
disassembly.

---

## See also

- [Hydraulic fundamentals](./01-hydraulics.md)
- [Mechanical seals](./03-seals.md)
- [pump-engineering-handbook §2 (gear)](https://github.com/fb-bombas/pump-engineering-handbook/tree/main/docs/02-gear)
