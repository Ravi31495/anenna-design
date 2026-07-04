# 📊 Results — Hairpin Bandpass Filter

## Simulation Environment

- **Software:** CST Studio Suite
- **Solver:** S-Parameter (Frequency Domain)
- **Sweep Range:** 3.6 GHz – 4.6 GHz

## Filter Geometry

![Hairpin filter geometry](images/filter_geometry.png)

*Two folded ("hairpin") microstrip resonator pairs, each consisting of two parallel strip arms connected at one end, arranged for edge-coupling between adjacent resonators.*

## S-Parameters (Magnitude)

![S-Parameters Magnitude](images/s_parameters.jpeg)

| Trace | Description |
|---|---|
| S1,1 (red) | Input return loss |
| S2,1 (green) | Forward transmission (overlaps closely with S1,2 in this sweep) |
| S1,2 (blue) | Reverse transmission |
| S2,2 (orange) | Output return loss |

### Key Observations

- **Return loss minima (S11):** sharp dips to below **-20 dB near 4.0 GHz**, and deeper nulls close to **-29 dB around 4.14 GHz** and **4.32 GHz** — indicating strong impedance matching at these frequencies.
- **Passband region:** Between roughly **4.1 GHz and 4.3 GHz**, S11/S22 drop sharply while transmission (S12) stays comparatively high (around -3 to -5 dB), consistent with a bandpass filter response centered in this range.
- **Out-of-band rejection:** Outside the passband (below ~3.9 GHz and above ~4.5 GHz), return loss rises toward 0 dB, showing increasing mismatch/rejection as expected for a bandpass structure.
- **Symmetry:** S11 and S22 (and S12/S21) traces are close to symmetric, suggesting a well-balanced, reciprocal two-port filter design.

## Conclusion

The hairpin filter demonstrates a clear bandpass characteristic centered around **4.1–4.3 GHz**, with two closely spaced resonant dips (4.14 GHz and 4.32 GHz) that likely correspond to the coupled-resonator pair. The design shows good matching (>20 dB return loss) at both resonances, validating the folded parallel-coupled-line approach for compact bandpass filtering.
