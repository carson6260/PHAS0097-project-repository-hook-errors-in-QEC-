# Quantum Error Correction — Circuit Generation and Simulation

This repository contains the Python functions and simulation notebooks used for my MSci dissertation on hook errors in quantum error correction.

The repository was created as a reference for the project report and contains the circuit-generation functions used to study the unrotated surface code and the 2D triangular colour code under different noise models.

## Circuit generation

`Circuit_generating_functions.ipynb` contains the three Python functions used to generate the circuits studied in the report:

* **Unrotated surface code — simple noise model:** includes a Pauli-X error on the ancilla after each CNOT.
* **Unrotated surface code — realistic circuit-level noise model:** includes the more realistic circuit-level noise model used in the report.
* **2D triangular colour code — realistic circuit-level noise model:** generates circuits for the Z-type stabilizers of the triangular colour code.

For the unrotated surface code, the CNOT operations are split across eight ticks, such that the X- and Z-type stabilizer measurements are not interleaved.

The triangular colour code function focuses on the Z-type stabilizers.

All circuit-generation functions support arbitrary CNOT gate orderings, allowing different schedules to be investigated.

## Simulation

`Stim_circuit_simulation(output_cleared).ipynb` contains the full simulation workflow used for the project, including the circuit generation, simulations, analysis and additional results that were not included in the final report.

The notebook has had its outputs cleared to reduce the file size for upload to GitHub.

## Dissertation

The full MSci dissertation is also available in this repository.

The dissertation investigates how CNOT gate ordering affects hook-error suppression in surface and triangular colour codes under different noise conditions.
