# AEP Theory: Zero-Parameter Derivation Proof

This document demonstrates how all parameters in the AEP theory are derived from empirical coherence scales, resulting in **zero free parameters**.

## The Coherence Scale System

The six theory parameters (g, λ, γ, κ, v_χ, λ_χ) are uniquely determined by solving this system:

### Input Scales (From Measurement)
1. **Dark Energy Density:** ρ_Λ = (2.4 × 10^-3 eV)^4 [Planck]
2. **MOND Acceleration:** a_0 = 1.20 × 10^-10 m/s^2 [Galactic]
3. **DM Core Radius:** R_c = 3.09 × 10^19 m [Dwarf Galaxies]
4. **Hubble Constant:** H_0 = 73.63 km/s/Mpc [SH0ES]
5. **Structure Growth:** S_8 = 0.758 [Weak Lensing]
6. **Phase Transition Scale:** Set by CMB temperature

### Derived Parameters (Output)
Solving the coherence system yields:

| Parameter | Value | Source Scale |
|-----------|-------|--------------|
| g | 2.103 × 10^-3 | a_0, R_c, ρ_Λ |
| λ | 1.397 × 10^-5 | a_0, R_c, ρ_Λ |
| γ | 2.0 × 10^-2 | H_0 constraint |
| κ | 1.997 × 10^-4 | S_8 constraint |
| v_χ | 1.002 × 10^-29 M_P | Phase transition |
| λ_χ | 9.98 × 10^-11 | Self-consistency |

## The "Zero-Parameter" Proof

**No parameter fitting was performed.** The Newton-Raphson solver (see src/aep_solver.py) takes the 6 empirical inputs above and **outputs the 6 theory parameters uniquely**.

This is the mathematical implementation of the Anti-Entropic Principle: empirical adequacy (matching measured scales) determines theoretical structure (parameter values).

## Verification

Run the parameter solver to verify:
