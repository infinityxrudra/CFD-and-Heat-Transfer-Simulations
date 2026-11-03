# CFD and Heat Transfer Simulations

### Numerical Methods | Computational Fluid Dynamics | Heat Transfer | Fluid Mechanics

A collection of **11 numerical simulation experiments** exploring fundamental and advanced concepts in Computational Fluid Dynamics (CFD), fluid mechanics, heat transfer, turbulence modelling, and numerical methods.

This repository demonstrates the application of computational techniques to engineering problems through Python-based numerical simulations, mathematical modelling, iterative solvers, and visualization of physical phenomena.

Each experiment includes:

* A Jupyter Notebook (`.ipynb`) containing the computational implementation.
* A PDF report documenting the objective, methodology, governing equations, simulation parameters, results, visualizations, and conclusions.

---

## Repository Overview

| Category                  | Details                                             |
| ------------------------- | --------------------------------------------------- |
| Total Experiments         | 11                                                  |
| Jupyter Notebooks         | 11                                                  |
| PDF Reports               | 11                                                  |
| Programming Language      | Python                                              |
| Computational Environment | Jupyter Notebook / Google Colab                     |
| Primary Domains           | CFD, Fluid Mechanics, Heat Transfer                 |
| Numerical Techniques      | Finite Difference, Finite Volume, Iterative Solvers |

---

# Experiments

## 1. External Flow over a NACA 0012 Airfoil

**Objective:** Simulate incompressible external flow over a NACA 0012 airfoil and investigate the influence of angle of attack on velocity, pressure distribution, wake structure, and aerodynamic characteristics.

**Simulation Parameters:**

* Reynolds Number: 100
* Angles of Attack: -5°, 0°, 5°, 10°
* Computational Grid: 120 × 60
* Total Iterations: 300

**Files:**

* [Jupyter Notebook](01_NACAAirfoil.ipynb)
* [PDF Report](Experiment1_23BME012.pdf)

---

## 2. Fluid Flow and Heat Transfer in a Double-Pipe Heat Exchanger

**Objective:** Investigate conjugate heat transfer between hot and cold laminar fluid streams separated by a conducting wall.

**Simulation Parameters:**

* Cold-stream Reynolds Numbers: 50, 100, 200
* Hot-stream Reynolds Number: 100
* Wall-to-fluid Heat Transfer Coefficient Ratios: 1 and 100
* Total Iterations: 3000

**Files:**

* [Jupyter Notebook](02_Double_Pipe_CHT_FDM.ipynb)
* [PDF Report](Experiment2_23BME012.pdf)

---

## 3. Internal Flow and Heat Transfer in a Centrifugal Pump

**Objective:** Study centrifugal pressure generation, velocity components, pump head, and temperature variation in a simplified rotating annular passage.

**Simulation Parameters:**

* Reynolds Number: 500
* Rotational Speeds: 1000, 2000, 3000 RPM
* Computational Grid: 80 × 160
* Total Iterations: 1200

**Files:**

* [Jupyter Notebook](03_Centrifugal_Pump_SRF.ipynb)
* [PDF Report](Experiment3_23BME012.pdf)

---

## 4. Kármán Vortex Shedding over a Circular Cylinder

**Objective:** Investigate unsteady flow past a circular cylinder and study the formation of alternating vortices in the wake. Estimate the Strouhal number associated with vortex shedding.

**Simulation Parameters:**

* Reynolds Number: 500
* Computational Grid: 80 × 160
* Total Iterations: 1200

**Files:**

* [Jupyter Notebook](04_Cylinder_Vortex_Shedding.ipynb)
* [PDF Report](Experiment4_23BME012.pdf)

---

## 5. Transient Couette Flow: Explicit and Implicit Formulations

**Objective:** Compare explicit FTCS and implicit Backward Euler numerical schemes for transient viscous momentum diffusion against the analytical solution.

**Simulation Parameters:**

* Kinematic Viscosity: 0.01
* Upper Plate Velocity: 1
* Grid Points: 81
* Final Simulation Time: 2
* Explicit Fourier Numbers: 0.25, 0.45, 0.55
* Implicit Fourier Number: 5

**Files:**

* [Jupyter Notebook](05_Transient_Couette_Flow.ipynb)
* [PDF Report](Experiment5_23BME012.pdf)

---

## 6. Two-Dimensional Plate Heat Conduction

**Objective:** Solve the steady two-dimensional Laplace equation and compare Jacobi and line-TDMA/SOR iterative solutions against an analytical solution.

**Simulation Parameters:**

* Fine Grid: 81 × 61
* Coarse Grid: 30 × 15
* Source Temperature: 100
* Maximum Iterations: 10,000
* Convergence Tolerance: 1 × 10⁻⁹

**Files:**

* [Jupyter Notebook](06_Plate_Conduction_2D.ipynb)
* [PDF Report](Experiment6_23BME012.pdf)

---

## 7. One-Dimensional Shallow-Water Wave

**Objective:** Compare first-order upwind and second-order Lax-Wendroff schemes for the propagation of a small-amplitude wave packet using the linearized shallow-water equations.

**Key Concepts:**

* Linearized shallow-water equations
* Conservative upwind scheme
* Lax-Wendroff numerical scheme
* CFL stability condition
* Numerical diffusion and dispersion
* Mass conservation

**Files:**

* [Jupyter Notebook](07_Shallow_Water_Wave.ipynb)
* [PDF Report](Experiment7_23BME012.pdf)

---

## 8. Rayleigh-Taylor Instability Using VOF-Style Modelling

**Objective:** Study the development of Rayleigh-Taylor instability at a perturbed interface between fluids of different densities using a bounded conservative volume-fraction transport model.

**Key Concepts:**

* Rayleigh-Taylor instability
* Volume-of-Fluid (VOF)-style modelling
* Boussinesq approximation
* Interface advection
* Volume-fraction boundedness
* Mass conservation

**Files:**

* [Jupyter Notebook](08_Rayleigh_Taylor_VOF.ipynb)
* [PDF Report](Experiment8_23BME012.pdf)

---

## 9. Lid-Driven Cavity Flow

**Objective:** Solve the incompressible lid-driven cavity flow problem using the vorticity-streamfunction formulation and analyse the formation of primary recirculation zones.

**Key Concepts:**

* Incompressible Navier-Stokes equations
* Vorticity-streamfunction formulation
* Streamfunction Poisson equation
* Successive Over-Relaxation (SOR)
* Wall-vorticity boundary conditions
* Recirculation and flow-field visualization

**Files:**

* [Jupyter Notebook](09_Lid_Driven_Cavity.ipynb)
* [PDF Report](Experiment9_23BME012.pdf)

---

## 10. Turbulent Pipe-Flow Model Comparison

**Objective:** Compare different radial eddy-viscosity closures for turbulent pipe flow by analysing velocity profiles, friction factors, pressure drop, and turbulent viscosity.

**Models Investigated:**

* Laminar flow model
* Mixing-length model
* Van Driest model
* Equilibrium k-epsilon closure
* Equilibrium k-omega / SST surrogate closure

**Key Concepts:**

* Turbulent pipe flow
* Eddy viscosity
* Velocity distribution
* Friction factor
* Pressure drop
* Turbulence modelling

**Files:**

* [Jupyter Notebook](10_Turbulent_Pipe_Models.ipynb)
* [PDF Report](Experiment10_23BME012.pdf)

---

## 11. Generic Convection-Diffusion Transport

**Objective:** Investigate scalar transport through convection and diffusion under different prescribed velocity fields, including forced flat-plate, forced-channel, and natural-convection surrogate cases.

**Key Concepts:**

* Convection-diffusion equation
* Scalar transport
* Finite-volume-style numerical formulation
* Forced convection
* Natural-convection surrogate modelling
* Transport phenomena

**Files:**

* [Jupyter Notebook](11_Convection_Diffusion.ipynb)
* [PDF Report](Experiment11_23BME012.pdf)

---

# Numerical Methods and Engineering Concepts

The repository covers a range of numerical techniques and engineering applications.

### Computational Fluid Dynamics

* Incompressible flow modelling
* External aerodynamics
* Internal and rotating flows
* Vortex shedding
* Lid-driven cavity flow
* Turbulent pipe-flow modelling
* Multiphase flow and interface transport

### Heat Transfer

* Conjugate heat transfer
* Two-dimensional steady-state conduction
* Transient heat and momentum diffusion
* Convection-diffusion transport

### Numerical Methods

* Finite Difference Method (FDM)
* Finite Volume-style formulations
* Explicit FTCS scheme
* Implicit Backward Euler scheme
* Lax-Wendroff scheme
* Upwind discretization
* Jacobi iterative method
* Line-TDMA and SOR
* Streamfunction-vorticity formulation
* Numerical stability and convergence analysis

---

# Tools and Technologies

| Tool / Technology | Application                                  |
| ----------------- | -------------------------------------------- |
| Python            | Numerical computation                        |
| NumPy             | Numerical arrays and mathematical operations |
| Matplotlib        | Scientific plotting and visualization        |
| Jupyter Notebook  | Computational implementation                 |
| Google Colab      | Cloud-based execution                        |
| GitHub            | Version control and project documentation    |

---


# Author

**Rudra Patel**
B.Tech – Mechanical Engineering,
Pandit Deendayal Energy University (PDEU), India

**Dr. Anirudh Kulkarni**
Assistant Professor - Mechanical Engineering,
Pandit Deendayal Energy University (PDEU), India
