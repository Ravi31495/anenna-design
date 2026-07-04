# 📡 Microstrip Patch Antenna Design (CST Studio Suite)

[![Tool](https://img.shields.io/badge/Simulated%20in-CST%20Studio%20Suite-1f6feb)]()
[![Band](https://img.shields.io/badge/Band-2.4%20GHz%20ISM-green)]()
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

A microstrip patch antenna designed and simulated in **CST Studio Suite**, targeting the **2.4 GHz ISM band** used in Wi-Fi, Bluetooth, and general wireless sensor applications.

## 📋 Table of Contents
- [Overview](#overview)
- [Design Specifications](#design-specifications)
- [Simulation Results](#simulation-results)
- [Repository Structure](#repository-structure)
- [Tools Used](#tools-used)
- [Future Work](#future-work)
- [License](#license)

## Overview

Microstrip patch antennas are widely used for their low profile, light weight, and ease of fabrication. This design was modeled and simulated in CST Microwave Studio to evaluate its gain, resonance, and radiation behavior around the 2.4 GHz ISM band.

## Design Specifications

| Parameter | Value |
|---|---|
| Design Software | CST Studio Suite |
| Target Frequency Band | 2.4 GHz (ISM) |
| Feeding Technique | Microstrip line feed |
| Substrate | *(update with material used, e.g. FR4 / Rogers RT5880)* |
| Simulated Peak Gain | ≈ 2.67 dB |

> Update the substrate/dielectric details above to match your exact `.cst` model parameters.

## Simulation Results

Full results with commentary are documented in **[RESULTS.md](RESULTS.md)**.

**Gain vs. Frequency (Phi = 0°):**

![Gain vs Frequency](images/gain_vs_frequency.jpeg)

The design achieves a peak gain of approximately **2.67 dB near 2.4 GHz**, with the gain curve rolling off symmetrically on either side of the resonant band — consistent with a single-band microstrip patch response.

## Repository Structure

```
├── README.md              # Project overview (this file)
├── RESULTS.md              # Detailed simulation results
├── CHANGELOG.md             # Version history
├── LICENSE
├── .gitignore
└── images/
    └── gain_vs_frequency.jpeg
```

## Tools Used

- **CST Studio Suite** (Microwave Studio) for EM simulation
- Far-field solver for gain/radiation pattern analysis

## Future Work

- [ ] Radiation pattern (2D/3D) analysis
- [ ] Bandwidth and VSWR optimization
- [ ] Array configuration for higher gain
- [ ] Fabrication and hardware validation

## License

Released under the [MIT License](LICENSE).
