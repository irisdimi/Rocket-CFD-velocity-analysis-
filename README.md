# Rocket CFD Velocity Analysis

**ENGG1800 Project 1**

## Overview

This project presents a Computational Fluid Dynamics (CFD) analysis of airflow around a rocket geometry, simulated in **Autodesk CFD 2024**. The main focus is **velocity magnitude**, visualised through contour planes at solver iterations 16, 49, and 62.

The simulation captures three key aerodynamic behaviours:
- Flow **acceleration** around the rocket body
- Local flow disturbance near the **fins**
- Formation of a **low-velocity wake region** behind the rocket

## Simulation Setup

- **Fluid:** Air
- **Rocket material:** Aluminium
- **Domain:** Rectangular air domain surrounding the rocket
- **Inlet:** Velocity-normal inlet condition
- **Outlet:** Gauge pressure condition, `p_out = 0 Pa`

The numerical model is based on conservation of mass (continuity equation) and momentum (Navier–Stokes equations), solved iteratively using the finite-volume method.

## Contents

- `BMET1800_CFD.pdf` — Full project report, including governing equations, numerical method, rocket nozzle simulation, and rocket body results
- Velocity contour images at iterations 16, 49, and 62

## Key Sections in the Report

1. **Simulation Overview** — domain setup and boundary conditions
2. **Governing Equations** — continuity, Navier–Stokes, Reynolds number, and Bernoulli's equation
3. **Numerical Method** — finite-volume discretisation and residual convergence
4. **Rocket Nozzle Simulation** — converging-diverging nozzle behaviour, choked flow at the throat, and thrust estimation
5. **Rocket Body CFD Results** — velocity contours at three solver iterations
6. **Discussion** — effects of the nose cone, fins, and wake formation on drag
7. **Key Aerodynamic Quantities** — summary table of velocity magnitude, dynamic pressure, Reynolds number, drag force/coefficient, and continuity

## Key Findings

- The **nose cone** smooths the incoming flow and reduces the stagnation region at the front of the rocket.
- The **fins** create local flow disturbances that contribute to drag.
- A **low-velocity wake** forms behind the rocket body as flow separates and loses momentum, contributing to pressure drag.
- As solver iterations progress (16 → 49 → 62), the velocity field becomes increasingly stable, indicating convergence.

## Tools Used

- Autodesk CFD 2024
- LaTeX (report typesetting)

## References

- Autodesk CFD 2024 simulation results generated for ENGG1800 Project 1
- ENGG1800 Project 1 CFD research notes
- Anderson, J. D. *Fundamentals of Aerodynamics*. McGraw-Hill.
- White, F. M. *Fluid Mechanics*. McGraw-Hill.
