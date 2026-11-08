# Data

## `chemotion_ir_processed.csv`

2,064 FT-IR spectra (mostly ATR) of 1,880 molecules, processed for machine learning.

**Source:** Chemotion Repository, *FT-IR spectroscopy data (Chemotion IR)*, [DOI: 10.22000/OGoEQGlsZGElrgst](https://doi.org/10.22000/OGoEQGlsZGElrgst). Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/); this processed version is shared under the same licence.

**Processing:** converted to absorbance, interpolated onto a common grid from 400 to 3996 cm⁻¹ in steps of 4 cm⁻¹ (900 points), and each spectrum scaled to lie between 0 and 1. Functional-group labels were assigned from the molecular structure (SMILES).

**Columns:**
* molecule information (including `smiles`);
* 15 functional-group labels (1 = present, 0 = absent): `carbonyl`, `ketone`, `aldehyde`, `ester`, `carboxylic_acid`, `amide`, `alcohol_phenol`, `amine_NH`, `nitrile`, `alkyne`, `alkene`, `aromatic`, `nitro`, `sulfonyl`, `halide`;
* 900 absorbance columns, named by wavenumber in cm⁻¹.

## `dls_silica_monodisperse.csv` (Lecture 1)

**Simulated** dynamic light scattering (DLS) correlation functions for silica particles in water at 298 K (viscosity 8.90 × 10⁻⁴ Pa s, refractive index 1.332, laser wavelength 633 nm), with Gaussian noise of standard deviation 0.005. The correlation function is the decay $g(\tau) = \beta\, e^{-D q^2 \tau}$ with $\beta = 0.9$, as in the colloids lecture notes.

Particles of diameter 30 nm, at 9 scattering angles. Columns: `tau_s` (lag time / s, 1 µs to 32 ms, log-spaced) and `g_30deg` … `g_150deg`.

Made by the lecturer for teaching; CC BY-SA 4.0 like the rest of the repository.
