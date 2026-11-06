# Data

## `chemotion_ir_processed.csv`

2,064 FT-IR spectra (mostly ATR) of 1,880 molecules, processed for machine learning.

**Source:** Chemotion Repository, *FT-IR spectroscopy data (Chemotion IR)*, [DOI: 10.22000/OGoEQGlsZGElrgst](https://doi.org/10.22000/OGoEQGlsZGElrgst). Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/); this processed version is shared under the same licence.

**Processing:** converted to absorbance, interpolated onto a common grid from 400 to 3996 cm⁻¹ in steps of 4 cm⁻¹ (900 points), and each spectrum scaled to lie between 0 and 1. Functional-group labels were assigned from the molecular structure (SMILES).

**Columns:**
* molecule information (including `smiles`);
* 15 functional-group labels (1 = present, 0 = absent): `carbonyl`, `ketone`, `aldehyde`, `ester`, `carboxylic_acid`, `amide`, `alcohol_phenol`, `amine_NH`, `nitrile`, `alkyne`, `alkene`, `aromatic`, `nitro`, `sulfonyl`, `halide`;
* 900 absorbance columns, named by wavenumber in cm⁻¹.
