# CFD and Heat Transfer Simulations

## Overview

This repository contains six numerical simulation experiments
covering Computational Fluid Dynamics (CFD), fluid mechanics,
heat transfer, and numerical methods.

The experiments investigate fluid flow around bodies, heat
transfer in engineering systems, vortex shedding, transient
momentum diffusion, and steady-state heat conduction.

Each experiment includes its objective, governing equations,
boundary conditions, numerical methodology, simulation
parameters, results, visualizations, and conclusions.

## Experiments

### Experiment 1: External Flow over a NACA 0012 Airfoil

**Objective:** To simulate incompressible external flow over
a NACA 0012 airfoil and investigate the influence of angle
of attack on velocity, pressure, wake structure, and qualitative
lift and drag trends.

**Key parameters:**
- Grid: 120 × 60
- Reynolds number: 100
- Angles of attack: -5°, 0°, 5°, and 10°
- Total iterations: 300

**Topics:** External aerodynamics, immersed-boundary methods,
pressure correction, vorticity, and aerodynamic force trends.


---

### Experiment 2: Fluid Flow and Heat Transfer in a Double-Pipe Heat Exchanger

**Objective:** To analyze conjugate heat transfer between hot
and cold laminar streams separated by a conducting wall.

**Key parameters:**
- Streamwise grid points: 160
- Cold-stream Reynolds numbers: 50, 100, and 200
- Hot-stream Reynolds number: 100
- Wall-to-fluid heat-transfer coefficient ratios: 1 and 100
- Total iterations: 3000

**Topics:** Conjugate heat transfer, convection-diffusion,
solid-wall conduction, temperature contours, and convergence.

---

### Experiment 3: Internal Flow and Heat Transfer in a Centrifugal Pump

**Objective:** To study centrifugal pressure rise, absolute
and relative velocities, pump head, and temperature variation
in a simplified rotating annular passage.

**Key parameters:**
- Coordinate system: Cylindrical
- Grid: 80 × 160
- Reynolds number: 500
- Pump speeds: 1000, 2000, and 3000 rpm
- Total iterations: 1200

**Topics:** Rotating flows, centrifugal pressure generation,
pump performance, thermal transport, and residual convergence.


---

### Experiment 4: Kármán Vortex Shedding over a Circular Cylinder

**Objective:** To resolve alternating vortex shedding behind
a circular cylinder and estimate the Strouhal number.

**Key parameters:**
- Coordinate system: Cylindrical
- Grid: 80 × 160
- Reynolds number: 500
- Total iterations: 1200

**Topics:** Lattice Boltzmann method, unsteady wakes, lift and
drag histories, vortex streets, and Strouhal number estimation.


---

### Experiment 5: Transient Couette Flow — Explicit and Implicit Formulations

**Objective:** To compare explicit FTCS and implicit backward-Euler
solutions of transient viscous momentum diffusion against
the analytical series solution.

**Key parameters:**
- Kinematic viscosity: 0.01
- Upper plate velocity: 1
- Grid points: 81
- Final simulation time: 2
- Explicit Fourier numbers: 0.25, 0.45, and 0.55
- Implicit Fourier number: 5

**Topics:** Numerical stability, time integration, Fourier number,
error analysis, and comparison with analytical solutions.


---

### Experiment 6: Two-Dimensional Plate Heat Conduction

**Objective:** To compare Jacobi and line-TDMA/SOR solutions
of the steady two-dimensional Laplace equation against
an analytical solution.

**Key parameters:**
- Fine grid: 81 × 61
- Coarse grid: 30 × 15
- Source temperature: 100
- Maximum iterations: 10000
- Convergence tolerance: 1 × 10^-9

**Topics:** Steady-state heat conduction, finite differences,
iterative solvers, convergence rate, and grid-size effects.


---

## Numerical Methods and Engineering Topics

The experiments cover the following methods and concepts:

- Incompressible Navier–Stokes equations
- Immersed-geometry projection methods
- Convection-diffusion and conjugate heat transfer
- Rotating-flow and centrifugal pressure models
- D2Q9 BGK lattice Boltzmann method
- Explicit FTCS and implicit backward-Euler schemes
- Jacobi and line-TDMA/SOR iterative methods
- Residual convergence and error analysis
- Velocity, pressure, temperature, and vorticity visualizations

## Repository Structure

```text
CFD-and-Heat-Transfer-Simulations/
│
├── README.md
│
├── Experiment-1-Airfoil/
│   └── Experiment1_23BME012.pdf
│
├── Experiment-2-Heat-Exchanger/
│   └── Experiment2_23BME012.pdf
│
├── Experiment-3-Centrifugal-Pump/
│   └── Experiment3_23BME012.pdf
│
├── Experiment-4-Vortex-Shedding/
│   └── Experiment4_23BME012.pdf
│
├── Experiment-5-Couette-Flow/
│   └── Experiment5_23BME012.pdf
│
└── Experiment-6-Heat-Conduction/
    └── Experiment6_23BME012.pdf
```

## Results and Documentation

Each experiment folder contains the corresponding PDF report
documenting the simulation setup, methodology, parameter
selection, numerical results, convergence behavior, and
engineering observations.

The repository is intended to provide an organized record
of numerical simulation work and its associated documentation.

## Author

**Rudra Patel**

B.Tech Mechanical Engineering

Pandit Deendayal Energy University (PDEU)

## Disclaimer

The reports document the numerical setups and results presented
in the respective experiments. Numerical values and conclusions
should be interpreted within the assumptions and limitations of
each simulation model.
