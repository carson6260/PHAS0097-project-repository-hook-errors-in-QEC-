# PHAS0097-project-repository-hook-errors-in-QEC-
The python functions used to generate the circuits used in the project.


This repository is used for referencing in the project report and contains the 3 python functions used in the project to generate the unrotated surface code under the simple noise model (only a pauli X error on the ancilla after each CNOT) and the more realistic circuit level noise model, and the 2D triangular colour code under realistic circuit level noise modoel. 


The CNOTs in the unrotated surface code is is split over 8 ticks (i.e. the X and Z stabilizers are not interleaved).


The triangular colour code function focuses on only the Z-type stabilizers. 


All functions support arbitrary gate orderings.


Circuit_generating_functions.ipynb has the 3 functions used to generate the circuits used for the report.



Stim_circuit_simulation(output_cleared).ipynb is the full file for the project and contains everything including those not included in the report (output has to be cleared to upload here, otherwise file size exceeds 25MB and can't upload).
