# Protoplanetary Disk Simulator

A modular, physics-based simulator for modelling the structure of protoplanetary disks around young stars.

This project aims to bridge the gap between simple textbook equations and large astrophysical modelling frameworks by providing an interactive and extensible implementation of the fundamental physics governing protoplanetary disks.

The primary goal is educational while remaining scientifically motivated, allowing users to visualize how changing stellar and disk parameters affects the resulting disk structure.

---

## Features

- Physics-based static protoplanetary disk model
- Modular pipeline architecture
- Parameter exploration
- 2D density structure visualization
- Radial profile analysis
- Vertical structure computation
- Temperature profile generation
- Surface density modelling
- Hydrostatic equilibrium solver
- Keplerian rotation calculations
- Optional gap/ring generation (future)
- Easily extendable for additional physics

---

## Physical Model

The simulator models a passive, flared protoplanetary disk using classical disk theory.

Current implementation includes

- Keplerian rotation
- Passive irradiation temperature profile
- Hydrostatic equilibrium
- Pressure scale height calculation
- Gaussian vertical density profile
- Self-similar surface density distribution
- Basic disk geometry

The implementation follows the simplified assumptions commonly adopted in modern disk modelling literature while avoiding computationally expensive radiative transfer and chemistry calculations.

---

## Current Assumptions

The baseline model assumes

- Geometrically thin disk
- Axisymmetric structure
- Static (time-independent) disk
- Hydrostatic equilibrium
- Passive stellar irradiation
- Vertically isothermal gas
- Keplerian rotation
- Constant mean molecular weight
- Well-mixed gas and dust
- Analytical surface density profile
- No chemistry
- No radiative transfer
- No magnetic fields
- No self-gravity
- No planet-disk interactions (baseline)

These assumptions allow rapid computation while reproducing the overall morphology of observed disks.

---

## Input Parameters

Typical model parameters include

### Stellar Parameters

- Stellar Mass
- Stellar Radius
- Stellar Luminosity
- Effective Temperature

### Disk Parameters

- Inner Radius
- Outer Radius
- Characteristic Radius
- Disk Mass
- Surface Density Index
- Temperature Power Law
- Reference Temperature
- Mean Molecular Weight

---

## Outputs

The simulator can generate

- Density maps
- Temperature profiles
- Scale height profile
- Surface density profile
- Midplane density
- Vertical density slices
- Keplerian velocity profile
- Aspect ratio (H/R)

Future versions will also support exporting simulation data for further analysis.

---

## Scientific Background

The project is inspired by the theoretical framework developed in

- Lynden-Bell & Pringle (1974)
- Shakura & Sunyaev (1973)
- Chiang & Goldreich (1997)
- Duffell (2015)
- Mordasini et al. (2014)

Rather than reproducing sophisticated radiative transfer codes, this project focuses on implementing the core physical equations in a transparent and educational manner.

---


## Example Workflow

```
Input Parameters
        │
        ▼
Surface Density
        │
        ▼
Temperature Profile
        │
        ▼
Scale Height
        │
        ▼
Vertical Density
        │
        ▼
Visualization
        │
        ▼
Interactive Dashboard
```

---

## Future Goals

The long-term vision is to develop a lightweight, modular platform where users can

- Explore the effects of disk parameters
- Compare theoretical models
- Reproduce characteristic disk morphologies
- Visualize astrophysical quantities interactively
- Serve as a foundation for more advanced protoplanetary disk simulations


