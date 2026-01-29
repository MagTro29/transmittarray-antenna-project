# HFSS Simulation Setup

This section documents the electromagnetic simulation setup used to
evaluate the filtering transmitarray antenna in **ANSYS HFSS**.

The simulations focus on validating unit-cell behaviour, frequency
response, and far-field radiation characteristics.

## Simulation Environment
- Simulator: ANSYS HFSS
- Frequency band of interest: Ku-band (~11.5–12.6 GHz)
- Analysis type: Frequency-domain EM simulation

## Unit Cell Modelling
The transmitarray is composed of magnetoelectric (ME) dipole unit cells.
Each unit cell is designed to provide one of two phase states (1-bit
quantisation) through physical rotation of the dipole structure.

Key modelling considerations include:
- Accurate substrate material properties
- Consistent unit cell periodicity
- Symmetry preservation for stable phase behaviour

## Boundary Conditions
To emulate an infinite periodic structure, appropriate boundary
conditions were applied:
- Periodic boundaries (master/slave or equivalent)
- Floquet port excitation for plane-wave incidence

These conditions allow evaluation of transmission magnitude and phase
response while reducing computational complexity.

## Excitation and Ports
The unit cell is excited using a plane wave source to analyse:
- Transmission coefficient (S21)
- Reflection coefficient (S11)
- Phase difference between the two unit-cell states

This approach enables direct comparison between the 0° and 180° phase
states required for 1-bit operation.

## Meshing and Accuracy
Adaptive meshing was used to ensure convergence across the operating
band. Mesh refinement focused on:
- Dipole edges
- Gaps and discontinuities
- Substrate interfaces

Convergence was verified by monitoring S-parameter stability across
multiple adaptive passes.
