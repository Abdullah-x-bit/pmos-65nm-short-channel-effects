# Deck → report map

Line numbers refer to `simulation/pmos_65nm_sce_analysis.in`.

| Deck lines | Section | Report topic (Phase 3) |
|-----------|---------|------------------------|
| 1-22 | Parameters, 65 nm scaling (k = 65/90) | Scaling of the device |
| 24-130 | Mesh, regions, electrodes, doping | PMOSFET structure |
| 131-166 | Materials, contacts, probes, Q<sub>ss</sub>, models, Newton method | n/a |
| 168-203 | I<sub>ds</sub>-V<sub>gs</sub> at V<sub>ds</sub> = −50 mV and −1.2 V; subthreshold swing | Transfer characteristics, operating regimes |
| 204-240 | I<sub>ds</sub>-V<sub>ds</sub> family (V<sub>gs</sub> = −0.5, −0.8, −1.0, −1.2 V) | Output characteristics, velocity saturation |
| 242-455 | Temperature sweep 300-550 K (V<sub>th</sub>, V<sub>fb</sub> extraction) | Temperature effects on V<sub>th</sub>, g<sub>m</sub>, r<sub>o</sub> |
| 456-492 | Gate-oxide tunneling (`qtnlsc.el/ho`) | Gate oxide tunneling |
| 493-529 | Equilibrium solution; I<sub>D</sub>-V<sub>DS</sub> at high V<sub>G</sub> and E-field at velocity saturation | CLM vs velocity saturation |
| 530-646 | I<sub>D</sub>-V<sub>GS</sub> at V<sub>D</sub> = −0.5…−3 V, E-field and band-diagram structure files | DIBL, field and band analysis |
| 647-691 | V<sub>TP0</sub> extraction (rest commented out) | DIBL quantification |
| 692-780 | C-V, high-frequency (AC) and low-frequency (QSCV) | C-V behavior |
| 781-841 | S/D junction depth sweep (commented out) | Scaling effects |
| 842-912 | μ<sub>eff</sub> extraction (commented out) | Effective mobility |
| 913-1107 | Duplicate commented-out block (NMOS-era names) | n/a |
| 1108-1130 | I<sub>on</sub> / I<sub>off</sub> extraction | On/off-current optimization |
