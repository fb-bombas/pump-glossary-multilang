# 6. Drivers, controllers, and instrumentation

## Electric motor

| PT | EN | ES |
|----|----|-----|
| Motor elétrico | Electric motor | Motor eléctrico |

Three-phase induction motors are the dominant pump driver. Key parameters:

- **Power rating** (kW or HP)
- **Voltage / frequency**: Brazil 220/380/440 V at **60 Hz**; Europe 400 V at 50 Hz; USA 460 V at 60 Hz
- **Service factor** (SF): typically 1.15 for industrial duty
- **Insulation class**: B (130 °C), F (155 °C), H (180 °C)
- **Efficiency class**: IE2 (high), IE3 (premium), IE4 (super premium)

**Gotcha:** **a 50 Hz motor running on 60 Hz overspeeds by 20%** — pump
flow goes up 20%, head up 44%, power up 73%. Imported pumps with 50 Hz-
design VFDs need careful re-rating in Brazil.

In Brazil, **IR2 / IR3** notation may also appear (older Eletrobras
classification, roughly equivalent to IE2 / IE3).

---

## Diesel engine driver

| PT | EN | ES |
|----|----|-----|
| Motor diesel | Diesel engine | Motor diésel |

Diesel-driven pumps are standard in fire-protection systems (NFPA 20,
NBR 16704) where electric power may fail during fire conditions.

Key requirements per NFPA 20:

- UL or FM listed for fire-pump duty
- Two battery banks, each capable of 1 hour cranking at 0 °C
- Fuel storage for **8 hours** of continuous full-load running
- Cooling water flow tested at idle and full load
- Engine overspeed shutdown

---

## Variable Frequency Drive (VFD)

| PT | EN | ES |
|----|----|-----|
| Inversor de frequência | Variable Frequency Drive (VFD) | Variador de frecuencia |

Power electronics that vary motor speed by varying supply frequency.
Allows the pump to follow varying process demand without throttling.

**Energy savings**: pump power scales with cube of speed (affinity laws).
Reducing speed 20% reduces power ~50%. Throttling a constant-speed pump
to achieve the same flow reduction wastes most of that power as
pressure drop.

**Gotcha:** VFDs introduce harmonics into the supply network. Per
ABNT NBR 5410 and IEC 61000, large pump installations may need harmonic
filters or 18-pulse / 24-pulse drive topologies.

---

## Soft starter

| PT | EN | ES |
|----|----|-----|
| Soft-starter / Partida suave | Soft starter | Arrancador suave |

Reduces motor inrush current during starting by ramping up voltage
gradually. Cheaper than a VFD and adequate where speed control is not
needed during operation.

**Gotcha:** soft starters do **not** provide ongoing speed control; they
only manage the start-up transient.

---

## Direct on Line (DOL)

| PT | EN | ES |
|----|----|-----|
| Partida direta | Direct on Line (DOL) | Arranque directo |

Simplest motor starting: contactor connects motor full-voltage. Inrush
current is 6-8× rated; mechanical shock to pump and driveline is high.

Acceptable for small pumps (typically < 5 kW) or where starts are
infrequent. Larger pumps use star-delta, soft starter, or VFD.

---

## Star-delta starter

| PT | EN | ES |
|----|----|-----|
| Partida estrela-triângulo | Star-delta starter | Arranque estrella-triángulo |

Older reduced-voltage starting method: motor windings connected in star
configuration during start (one-third inrush), then switched to delta for
running. Gradually displaced by soft starters for new installations.

---

## Pressure switch

| PT | EN | ES |
|----|----|-----|
| Pressostato | Pressure switch | Presostato |

Mechanical or electronic device that triggers a contact closure when
fluid pressure crosses a setpoint. Common pump-control uses:

- Start main pump on system-pressure drop
- Stop / start jockey pump on small pressure variations
- Low-pressure alarm
- High-pressure shutdown

In fire-pump applications (NFPA 20 §10.5), pressure-switch setpoints are
strictly defined to prevent the main pump from short-cycling.

---

## Flow switch

| PT | EN | ES |
|----|----|-----|
| Chave de fluxo / Fluxostato | Flow switch | Interruptor de flujo |

Triggers contact closure on presence or absence of flow. Used for pump
dry-running protection — if process flow stops while pump runs, the flow
switch shuts the pump down before the seal burns.

**Gotcha:** flow switches must be sized for the minimum-flow point, not
the rated point. A switch that triggers at 30% rated flow will not protect
during slow-leak scenarios.

---

## Automatic Transfer Switch (ATS)

| PT | EN | ES |
|----|----|-----|
| Chave de transferência automática | Automatic Transfer Switch (ATS) | Conmutador automático |

Automatically transfers electrical load between two power sources
(typically utility and standby generator) when one fails. Standard
component in fire-pump electrical systems and in critical-process
pumping systems with backup generation.

UL 1008 is the listing standard for fire-pump ATS.

---

## SCADA

| PT | EN | ES |
|----|----|-----|
| SCADA / Supervisão e controle | SCADA / Supervisory Control | SCADA / Supervisión y control |

Supervisory Control and Data Acquisition. Software platform that
collects pump operating data (flow, pressure, temperature, vibration)
from instruments and displays it to operators. Common in industrial
plants with 50+ pumps where centralized monitoring saves walking time.

---

## Protocol — fieldbus

Common industrial protocols for pump instrumentation:

- **Modbus RTU** (RS-485): widespread, simple, well supported
- **Modbus TCP**: Modbus over Ethernet
- **Profibus DP**: European industrial standard; declining for new installations
- **Profinet**: Profibus successor over Ethernet
- **HART**: superimposed digital signal on 4-20 mA analog loops
- **Foundation Fieldbus**: ABB / Emerson / Honeywell preferred for critical-loop instruments

Pump-side instruments (pressure, temperature, vibration) typically
communicate via Modbus RTU or HART; controller-side communication is
usually Profinet or Modbus TCP.

---

## Vibration monitoring

| PT | EN | ES |
|----|----|-----|
| Monitoramento de vibração | Vibration monitoring | Monitoreo de vibración |

Real-time or periodic measurement of bearing-housing vibration to detect
emerging mechanical issues. Critical pumps often have permanent
accelerometers feeding a condition-monitoring system; smaller pumps use
periodic walk-around vibration meters.

Per ANSI/HI 9.6.4:

- Velocity RMS ≤ 5.0 mm/s for pumps ≤ 1.800 rpm
- Velocity RMS ≤ 7.1 mm/s for pumps > 1.800 rpm

Measured in the radial direction at each bearing housing.

---

## See also

- [Standards](./05-standards.md)
- [Failure modes](./07-failure-modes.md)
