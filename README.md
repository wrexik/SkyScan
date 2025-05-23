# SkyScan
An autopilot 4'' FPV drone with INAV and OpenIPC used for photogrametry!

---

## Table of Ideas
- Under 250g
- 4" frame
- Digital FPV with OpenIPC
- INAV - GPS and Mission planning
- 4S battery

## Conectivity
- OpenIPC - 2.4GHz > Realtime HD video
- ELRS - 900MHz > Long range control
- GPS - 1.5GHz > Location & telemetry

# Hardware

  | **Component**                     | **Model / Specs**                                                       | **Notes**                         |
|----------------------------------|--------------------------------------------------------------------------|-----------------------------------|
| **Frame**                        | JMT LR4 169mm 4" Frame Kit                                               | ~50g, supports 20x20, 25.5x25.5mm |
| **Flight Controller + ESC**      | Speedybee F405 AIO 40A (25.5x25.5mm)                                     | BLHeli_32, Bluejay, 3–6S support  |
| **Motors**                       | 4x T-Motor P1604 3800KV                                                  | 4S optimized, 9x9mm mount         |
| **Receiver**                     | Radiomaster XR1 Nano Dual-Band ELRS 2.4GHz + 900MHz                      | High range redundancy             |
| **Radio Controller**             | Radiomaster Pocket (TC-style with built-in ELRS 2.4GHz)                  | No external module required       |
| **Camera & VTX**                 | EMAX Wyvern Link Alpha (OpenIPC support, 5.8GHz HD, 100mW)               | OpenIPC-compatible                |
| **Props**                        | Gemfan Hurricane 4023 / HQProp T4x2.5x3                                  | For 4" efficiency/freestyle       |
| **Battery (light)**              | 4S 850mAh Li-ion                                                         | Sub-250g compatible               |
| **Battery (long range)**         | 4S 18650 3000mAh Li-ion (e.g., VTC6 pack)                                | Up to 40+ min flight              |