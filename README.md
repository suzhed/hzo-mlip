# HfₓZr₁₋ₓO₂ Deep Potential Project

This repository contains Deep Potential (DP) models, training datasets, and computational files for HfₓZr₁₋ₓO₂ (HZO) solid solutions, with a focus on structural properties, dielectric response, phase stability, and phase transitions.

## File Description

### `dp_run/`

Input files for iterative Deep Potential model training using DP-GEN and DeepMD-kit.

The directory contains the following main files:

* `param.json`: Main DP-GEN parameter file defining the iterative training workflow.
* `machine.json`: Machine configuration file for DP-GEN calculations.
* `INCAR_scf`: VASP INCAR template for self-consistent first-principles calculations.
* `POTCAR_Hf`, `POTCAR_Zr`, and `POTCAR_O`: VASP PAW potential files for Hf, Zr, and O, respectively.
* `dpgen.log`: Log file generated during the DP-GEN iterative training workflow.

### `HZO_model.pb`

Trained Deep Potential model for HfₓZr₁₋ₓO₂ solid solutions. The neural-network architecture and training parameters are specified in `./dp_run/param.json`.

### `dataset.tar.gz`

Training and testing datasets containing atomic configurations of HZO with different compositions, crystal structures, temperatures, and pressures.

The dataset includes monoclinic (m), tetragonal (t), orthorhombic-1 (o1), and orthorhombic-3 (o3) phases.

### `hzo_eps.tar.gz`

Computational and analysis files for finite-temperature simulations of dielectric properties in different HZO phases and the temperature-driven o3–t phase transition.

### `hzo_o3-t.tar.gz`

Computational files for investigating the temperature-driven o3–t phase transition in HZO.

### `phase_diagram.tar.gz`

Computational files for constructing the ZrO₂ phase diagram using thermodynamic integration and the two-phase coexistence method.

### `test.tar.gz`

Files for testing and validating the Deep Potential model, including calculations of elastic properties, enthalpy, equation of state (EOS), structural optimization, and phonons, as well as convergence and model tests.
