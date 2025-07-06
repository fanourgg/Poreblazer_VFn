# Modified PoreBlazer

This repository contains a modified version of [PoreBlazer v3.0.5]("https://github.com/richardjgowers/poreblazer").

### Summary of Changes

This version computes together with the Helium Void Fraction (VF) its second,
third and fourth non-central moments (denoted as VF2, VF3 and VF4,
respectively). These calculations require only minimal changes of the original
source codes.

### Original Source

The original code was obtained from the official GitHub repository:  
https://github.com/richardjgowers/poreblazer

We thank the developers for making their work openly available.

### What’s Included Here

- `poreblazer_VFn/` — It contains everything is included in the original
version. However, inside the directory with the source files there are few
modifications in the `poreblazer.f90` fortran code needed for the calculation
and the printout of the VF1, VF2, VF3, VF4. The original version of the
`poreblazer.f90` is also included in there (renamed to
`poreblazer_original.f90`) but is not used.

- `examples_VFn/` test files and example outputs of the modified version of
poreblazer for the `ABEXEM_clean.cif` (directory `ABEXEM/`) and the
`CIXCAR_clean.cif` (directory `CIXCAO/`) MOFs. The various input files are the
same as in the two version. The output of the new version with respect to the
original one differs only in the printout of the VF1 (=void fraction) VF2, VF3
and VF4. For the previous examples these values are (see the output files):

  - **ABEXEM_clean**  
    VF1: 0.343  
    VF2: 0.808  
    VF3: 2.143  
    VF4: 6.287
  - **CIXCAO_clean**  
    VF1: 0.617  
    VF2: 1.220  
    VF3: 2.678  
    VF4: 6.381

- `README_VFn.md` — this file describing the modifications

### Notes

This version was used for the calculation of the MOFs void fraction and the
VFn=(VF2, VF3 and VF4) Machine Learning descriptors of the manuscript: "A
Physically Motivated Machine Learning Model for Accurate Gas Adsorption
Predictions in Nanoporous Materials" by L. Manitsas and G. S.  Fanourgakis.  If
you use or adapt this version, please cite the original PoreBlazer publication
alongside our work.

- `Sarkisov and Harrison, Computational structure characterisation tools in 
application to ordered and disordered porous materials, Molecular 
Simulation, Vol 37, Issue 15, pages 1248-1257, 2011.
