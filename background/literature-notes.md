# Background and Literature Notes

This project is based on the concept of a **filtering transmitarray antenna**
using **magnetoelectric (ME) dipole elements** to achieve radiation and
frequency selectivity within a single structure.

Transmitarray antennas (TAs) offer an alternative to traditional reflector
and phased-array antennas by using a planar array of unit cells to control
the transmitted wavefront. Compared to conventional phased arrays, TAs can
reduce feed complexity and RF losses.

## Magnetoelectric Dipole Concept
ME dipole antennas combine electric and magnetic dipole characteristics,
allowing for:
- Wide impedance bandwidth
- Stable radiation patterns
- Improved polarization performance

In this project, the ME dipole structure enables both radiation and filtering
behaviour, reducing the need for external RF filtering stages.

## 1-bit Phase Quantisation
The transmitarray implements **1-bit phase control**, where each unit cell
provides one of two phase states. Phase control is achieved through physical
rotation of the ME dipole element, simplifying the design while maintaining
acceptable beamforming performance.

Although higher-bit quantisation can improve beam accuracy, 1-bit designs
offer a strong trade-off between performance, complexity, and manufacturability.

## Filtering Transmitarray Architecture
Unlike conventional TAs, the filtering transmitarray integrates frequency
selective behaviour directly into the unit cell design. This improves
out-of-band suppression and system-level efficiency.

The design aligns with modern RF system requirements where antenna and filter
co-design is increasingly important.
