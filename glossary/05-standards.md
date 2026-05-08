# 5. Standards and certifications

## ISO 2858

End-suction centrifugal pumps — designation, nominal duty point, and
dimensions. Rates the pump for 16 bar at 20 °C as a baseline.

European-origin standard, widely adopted internationally including Brazil
where ABNT references it. The dimensional standard fixes baseplate
mounting, suction/discharge nozzle sizes, and flange dimensions, but does
not fix hydraulic performance.

**Gotcha:** "compliance with ISO 2858" is a **dimensional** claim, not a
performance claim. Two ISO-2858 pumps in the same size class will fit on
the same baseplate but produce different curves.

---

## ASME B73.1

Specification for horizontal end-suction centrifugal pumps for chemical
process. North American counterpart to ISO 2858, with similar
dimensional fixity but different size matrix.

ASME B73.2 covers vertical in-line versions. ASME B73.3 covers sealless
(magnetic-drive) variants.

---

## API 610

Centrifugal pumps for petroleum, petrochemical, and natural gas
industries. Heavy-duty process-pump standard with stricter casing,
bearing, and seal requirements than general-industrial pumps. API 610
pumps are typically more expensive but designed for 5+ years of
continuous service in hydrocarbon duty.

Current edition: API 610 12th edition (2021).

**Gotcha:** API 610 specifies pump types by letter code (OH1 through
OH3, BB1 through BB5, VS1 through VS7). "API 610 OH2" means
overhung-impeller, foot-mounted, single-stage centrifugal — the most
common type in refining service.

---

## API 676

Positive-displacement pumps — rotary. Covers gear, lobe, screw, and
sliding-vane pumps for petroleum service.

---

## API 682

Pumps — shaft sealing systems for centrifugal and rotary pumps. Defines
seal arrangements (1, 2, 3) and support-system plans (Plan 11, 13, 21,
23, 32, 52, 53, 54, etc.). Cross-referenced from API 610 and API 676.

---

## ANSI/HI 14.6

Rotodynamic pumps for hydraulic performance acceptance tests. Defines
test methodology, instrumentation accuracy, and tolerance bands by
acceptance grade:

| Grade | Application | Q tolerance | H tolerance |
|-------|-------------|-------------|-------------|
| 1U | API duty | ±5% | ±3% |
| 1B | Industrial standard | ±8% | ±5% |
| 2B | Commercial / utility | ±10% | ±8% |
| 3B | Light duty | ±10% | ±8% |

Current edition: ANSI/HI 14.6-2022.

---

## ANSI/HI 9.6.1, 9.6.3, 9.6.4

Hydraulic Institute reliability and operating-region standards:

- **9.6.1**: NPSH margin requirements
- **9.6.3**: Allowable operating region (70-110% BEP for centrifugal)
- **9.6.4**: Vibration limits

These are not separate certifications — they are referenced by API 610,
HI 14.6, and pump-supply contracts as the operating envelope.

---

## ISO 9906

Rotodynamic pumps — Hydraulic performance acceptance tests, Grades 1, 2,
and 3. International equivalent of ANSI/HI 14.6 with similar but not
identical tolerance bands.

Current edition: ISO 9906:2012.

---

## NFPA 20

Standard for the Installation of Stationary Pumps for Fire Protection.
US National Fire Protection Association standard, widely adopted
internationally. Defines pump performance envelope (65/100/140 rule),
controller requirements, jockey-pump arrangement, and field-acceptance
testing.

Current edition: NFPA 20: 2025.

---

## ABNT NBR 16704

Bombas para combate a incêndio — Requisitos. Brazilian fire-pump
standard. Harmonized with NFPA 20 with Brazil-specific additions for
documentation language, INMETRO certification chain, and Bombeiros field-
acceptance procedure.

Current edition: NBR 16704:2020.

See [`fb-bombas/nfpa20-fire-pump-checklist`](https://github.com/fb-bombas/nfpa20-fire-pump-checklist)
for clause-by-clause comparison.

---

## ABNT (Associação Brasileira de Normas Técnicas)

Brazilian standards body. Issues NBR-prefixed standards. Pump-related NBRs
include NBR 16704 (fire), NBR 12515 (terminology), NBR 13929
(mechanical seals), and several others.

Standards are in **Portuguese**; English translations are not
authoritative.

---

## INMETRO

Instituto Nacional de Metrologia, Qualidade e Tecnologia. Brazilian
metrology authority. Recognizes laboratories, accredits certification
bodies, and operates the SBAC (Sistema Brasileiro de Avaliação da
Conformidade).

For fire pumps and other regulated products, **INMETRO-recognized lab
certificates** are required for Brazilian acceptance. International
certificates (UL, FM, TÜV) are usable when the issuing lab is on
INMETRO's mutual-recognition list.

---

## CRCC Petrobras

Cadastro Corporativo de Fornecedores. Petrobras' qualified supplier
registry. Vendors selling to Petrobras must hold current CRCC
registration for the relevant product family. Registration audits both
technical capability (testing, manufacturing, quality control) and
financial-statement reliability.

A CRCC entry is a meaningful **Tier-1-vendor** signal in Brazilian
oil-and-gas procurement. Non-Petrobras buyers in similar industries often
treat CRCC registration as a positive screen.

---

## CE marking

European Conformity. Mandatory marking for products sold in the European
Economic Area, indicating compliance with applicable directives (Pressure
Equipment Directive 2014/68/EU, Machinery Directive 2006/42/EC, etc.).

**Gotcha:** CE marking is **self-declared** for most pump categories,
not third-party certified. The presence of CE marking does not
substitute for a manufacturer's quality reputation or test certificates.

---

## UL listing / FM approval

Underwriters Laboratories listing and Factory Mutual approval are US
listings widely recognized internationally for fire-protection
equipment. UL 448 covers fire-pump centrifugal pumps; FM Class 1319
covers fire pumps under FM rules.

For NBR 16704 acceptance, UL or FM listing is generally accepted with
INMETRO-mutual-recognition cross-check.

---

## See also

- [Hydraulic fundamentals](./01-hydraulics.md) — for HI 14.6 tolerance application
- [pump-engineering-handbook §4 (fire-fighting)](https://github.com/fb-bombas/pump-engineering-handbook/tree/main/docs/04-fire-fighting)
- [`fb-bombas/nfpa20-fire-pump-checklist`](https://github.com/fb-bombas/nfpa20-fire-pump-checklist)
