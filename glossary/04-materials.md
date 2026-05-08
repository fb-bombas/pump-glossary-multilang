# 4. Materials and corrosion

## Cast iron

| PT | EN | ES |
|----|----|-----|
| Ferro fundido (cinzento) | Cast iron / Gray iron | Hierro fundido / Hierro gris |

Iron-carbon alloy with carbon as graphite flakes. Inexpensive, easy to
cast, good vibration damping. Used for non-corrosive water service at
moderate temperatures (< 100 °C) and pressures.

**Gotcha:** plain cast iron is **not suitable** for thermal-oil pumps
(temperature) or fire-pump casings (pressure rating + impact resistance).
Specify ductile iron or cast steel for those.

---

## Ductile iron (nodular cast iron)

| PT | EN | ES |
|----|----|-----|
| Ferro fundido nodular / Ferro dúctil | Ductile iron / Nodular cast iron | Hierro dúctil / Hierro fundido nodular |

Cast iron with magnesium addition that turns the graphite from flakes to
spheroids. Roughly 3× tensile strength and substantially higher impact
resistance than gray cast iron. Common upgrade material for casings
exposed to thermal cycling or shock loading.

ASTM A536 is the typical grade designation; common types include 60-40-18
and 65-45-12.

---

## Cast steel

| PT | EN | ES |
|----|----|-----|
| Aço fundido | Cast steel | Acero fundido |

Carbon or low-alloy steel cast into pump casings. Used where pressure,
temperature, or impact requirements exceed ductile iron. Standard grade
for API 610 process pumps (typically WCB or WCC per ASTM A216).

---

## Stainless steel — austenitic (300 series)

| PT | EN | ES |
|----|----|-----|
| Aço inoxidável austenítico | Austenitic stainless steel | Acero inoxidable austenítico |

Iron-chromium-nickel alloys, typically 18% Cr / 8% Ni base (304) or with
molybdenum addition for chloride resistance (316). Non-magnetic, ductile,
good general corrosion resistance.

| Grade | Composition | Where used |
|-------|------------|------------|
| 304 / 1.4301 | 18% Cr, 8% Ni | General mild service |
| 304L / 1.4307 | low-carbon variant | Welded fabrications |
| 316 / 1.4401 | + 2-3% Mo | Chloride-bearing fluids |
| 316L / 1.4404 | low-carbon | Welded chloride service |
| 321 / 1.4541 | + Ti stabilizer | High-temperature service (550-800 °C) |

**Gotcha:** 304 is **not** chloride-resistant. Sea water, brackish water,
and chlorinated cooling water need 316 minimum, often duplex.

---

## Duplex and super-duplex stainless

| PT | EN | ES |
|----|----|-----|
| Aço inoxidável duplex / super-duplex | Duplex / super-duplex stainless steel | Acero inoxidable dúplex / súper dúplex |

Stainless steels with mixed austenite-ferrite microstructure. Roughly 2×
yield strength of 316 and superior chloride / pitting resistance.

| Grade | PREN range | Where used |
|-------|-----------|-----------|
| 2205 / 1.4462 | ~ 35 | Standard duplex; sea-water at moderate temperature |
| 2507 / 1.4410 | ~ 42 | Super-duplex; warm sea-water, brackish, sulfur-containing fluids |

PREN = Pitting Resistance Equivalent Number = %Cr + 3.3 × %Mo + 16 × %N.
PREN > 40 is the typical super-duplex threshold.

---

## Hastelloy

| PT | EN | ES |
|----|----|-----|
| Hastelloy | Hastelloy | Hastelloy |

Family of nickel-based alloys (Haynes International trademark) for severe
corrosive service. Common grades:

| Grade | Resistant to |
|-------|--------------|
| Hastelloy B-3 | Concentrated hydrochloric acid |
| Hastelloy C-22 | Oxidizing chlorides, mixed acids |
| Hastelloy C-276 | Wet chlorine, hypochlorites, complex chlorinated solvents |

Cost is typically 8-15× the cost of 316 stainless. Used only where
cheaper materials cannot survive.

---

## CD4MCu (cast duplex)

| PT | EN | ES |
|----|----|-----|
| CD4MCu | CD4MCu | CD4MCu |

ASTM A890 cast duplex stainless. Common in pump impellers and casings for
pulp & paper, mining, and chemical service. Roughly equivalent corrosion
resistance to wrought 2205 with the casting-friendly composition.

---

## Bronze (gunmetal, naval bronze)

| PT | EN | ES |
|----|----|-----|
| Bronze (canhão / náutico) | Bronze (gunmetal / naval) | Bronce (de cañón / naval) |

Copper-tin alloys, sometimes with zinc, lead, or nickel additions. Used
for sea-water pump impellers (B62 gunmetal), marine fittings, and
applications where the material must be non-sparking.

**Gotcha:** bronze is dezincified by some chloride-bearing waters,
especially soft acidic waters. For hot or acidic sea-water service,
specify duplex or higher-grade alloys.

---

## Elastomers (O-rings and gaskets)

| PT | EN | ES |
|----|----|-----|
| Elastômeros (anéis O-ring e juntas) | Elastomers (O-rings and gaskets) | Elastómeros (juntas tóricas y juntas) |

| Material | Temperature range | Resistant to | Avoid |
|----------|-------------------|--------------|-------|
| NBR (Buna-N) | -30 to +100 °C | Petroleum oils, water | Polar solvents, ozone |
| EPDM | -40 to +150 °C | Hot water, steam, weak acids | Petroleum oils, fuels |
| FKM (Viton) | -20 to +200 °C | Most chemicals, oils, fuels | Hot amines, MEK, esters |
| FFKM (Kalrez) | -20 to +325 °C | Almost everything | Cost (10-30× FKM) |
| PTFE | -200 to +260 °C | Almost everything | Mechanical creep |
| Aflas | -10 to +230 °C | Amines, sour gas, acids | Cost |

**Gotcha:** "Viton" is a Chemours trademark for a specific FKM grade
family. Generic FKM is the correct technical term. PT and ES catalogs use
"Viton" loosely as a synonym for FKM, which can produce procurement
mismatches between buyer and vendor.

---

## See also

- [Pump types](./02-pump-types.md)
- [Mechanical seals](./03-seals.md)
