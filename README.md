# Pump Glossary — Trilingual (PT / EN / ES)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC--BY--4.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)

A working trilingual reference of industrial pump terminology — Portuguese,
English, Spanish — written for engineers, buyers, and translators who need
to navigate pump documentation across Brazilian, North American, and
Latin American suppliers.

Every entry has:

- The term in PT / EN / ES
- A precise definition
- A "why it matters" or "common gotcha" note
- A link to the relevant standard or pump-engineering reference

This is not a translation table. It is an opinionated reference written to
catch the places where literal translation produces engineering errors.

CC BY 4.0 — copy, adapt, redistribute with attribution to **FB Bombas**.

---

## Contents

- [Hydraulic fundamentals](./glossary/01-hydraulics.md) — flow, head, NPSH, BEP
- [Pump types](./glossary/02-pump-types.md) — centrifugal, gear, axial, lobe, diaphragm
- [Mechanical seals and shaft sealing](./glossary/03-seals.md) — single, dual, packing, magnetic drive
- [Materials and corrosion](./glossary/04-materials.md) — cast iron, duplex, hastelloy, elastomers
- [Standards and certifications](./glossary/05-standards.md) — API, ISO, ANSI/HI, NFPA, NBR
- [Drivers, controllers, and instrumentation](./glossary/06-drivers-controls.md) — VFDs, soft starters, ATS, pressure switches
- [Failure modes](./glossary/07-failure-modes.md) — cavitation, recirculation, dry-running, water hammer

Total: ~60 terms across the seven sections. Each section is self-
contained — read in any order.

---

## How this glossary is different

Most pump glossaries are translation tables. They translate "centrifugal
pump" to "bomba centrífuga" and stop.

The problem: Brazilian, Mexican, and Argentine engineers use the same
words for **subtly different concepts** — and getting those distinctions
wrong creates real engineering errors.

A few examples we cover:

- **"Cabeça" vs "altura manométrica" vs "head"**: All three are used
  interchangeably in casual Portuguese, but ABNT prefers "altura
  manométrica" and "head" is the international term. In a contract,
  pick one and be consistent.
- **"Selo mecânico" vs "vedação mecânica"**: Both appear in Brazilian
  practice but ABNT NBR 13929 standardized "vedação mecânica" — most
  vendor catalogs still use "selo mecânico". Either is acceptable in
  technical writing; "vedação" is more correct.
- **"Cavitación" (ES) vs "cavitação" (PT)**: Same phenomenon, but the
  Spanish term sometimes gets translated to English as "caving in"
  instead of "cavitation" — a category error.
- **"NPSH disponible / disponível / available"**: All correct. But the
  abbreviation "NPSH-d" appears in some Spanish-language contracts;
  "NPSHa" is the international convention.

This glossary explicitly notes these distinctions where they matter.

---

## About FB Bombas

[FB Bombas](https://www.fbbombas.com.br) — Brazilian industrial pump
manufacturer in Cabreúva, São Paulo, since 1944. Trilingual catalog
covering centrifugal, gear, thermal-oil, and fire-fighting pumps for
Brazilian and Latin American markets.

The full FB Bombas trilingual glossary lives at:

- Portuguese: [`/glossario`](https://www.fbbombas.com.br/glossario)
- English: [`/en/glossary`](https://www.fbbombas.com.br/en/glossary)
- Spanish: [`/es/glosario`](https://www.fbbombas.com.br/es/glosario)

This repository is a curated subset — the terms most useful for
cross-language procurement, specification, and technical translation.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Copy, adapt,
redistribute with attribution to **FB Bombas**.

## Contributing

Spotted a translation error? A regional usage we missed? Open an issue
or PR. Brazilian, Argentine, Mexican, Chilean, Colombian, Peruvian
regional usage all welcome — note your regional context.


---

## More from the FB Bombas open knowledge base

All knowledge-base sites are hosted on GitHub Pages and licensed under
CC BY 4.0 (or CC BY-ND 4.0 for the manuals mirror).

- [`pump-engineering-handbook`](https://fb-bombas.github.io/pump-engineering-handbook/) — Open knowledge base on industrial pumping fundamentals — centrifugal, gear, thermal-oil, fire-fighting
- [`nfpa20-fire-pump-checklist`](https://fb-bombas.github.io/nfpa20-fire-pump-checklist/) — 47-item NFPA-20 / NBR-16704 fire-pump compliance checklist
- [`pump-procurement-playbook`](https://fb-bombas.github.io/pump-procurement-playbook/) — Industrial pump procurement playbook — RFQ, TCO, contract clauses
- [`latam-pump-buyers-guide`](https://fb-bombas.github.io/latam-pump-buyers-guide/) — Country-by-country LATAM procurement guide — Brazil, Mexico, Argentina, Chile, Colombia, Peru
- [`fb-bombas-technical-manuals`](https://fb-bombas.github.io/fb-bombas-technical-manuals/) — Official FB Bombas technical manuals (PDF) — FBCN, FBE, FBEI, FBOT

Canonical FB Bombas: [www.fbbombas.com.br](https://www.fbbombas.com.br) · [Manuais técnicos](https://www.fbbombas.com.br/manuais-tecnicos)
