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

## `coffee_ftir_spectra.csv` (Lecture 2)

56 mid-infrared diffuse reflectance (DRIFT) FTIR spectra of freeze-dried instant coffee: 29 Arabica and 27 Robusta (*Coffea canephora* var. robusta), 286 points from 810.548 to 1910.644 cm⁻¹ (spacing 3.86 cm⁻¹).

**Source:** Quadram Institute Bioscience (formerly Institute of Food Research), [example data sets](https://csr.quadram.ac.uk/example-datasets-for-download/), file `FTIR_Spectra_instant_coffee.csv`, made available under the BBSRC data-sharing policy (free to analyse and redistribute with acknowledgement). Described in R. Briandet, E. K. Kemsley and R. H. Wilson, *J. Agric. Food Chem.* **44**, 170–174 (1996), [doi:10.1021/jf950305a](https://doi.org/10.1021/jf950305a), and G. Downey, R. Briandet, R. H. Wilson and E. K. Kemsley, *J. Agric. Food Chem.* **45**, 4357–4361 (1997).

**Processing:** none apart from layout: the original file has one spectrum per column; here there is one spectrum per row. Columns: `sample` (original sample number), `species` (`Arabica` or `Robusta`), then 286 intensity columns named by wavenumber in cm⁻¹ (units as in the original file).
