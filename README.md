# Advanced Physical Chemistry: Machine Learning in Chemistry

Notebooks and data for the six-lecture *Machine Learning in Chemistry* course  part of Advanced Physical Chemistry, University of Edinburgh, 2026/27.

Lecturer: Dr Antonia Mey (antonia.mey@ed.ac.uk)

## Contents

There is one folder per lecture. Only the Lecture 4 notebook is required other are optional extras for practice.

| Lecture | Topic | Notebook | |
|---|---|---|---|
| L1 | From fitting to learning | [`L1_fitting/L1_fitting_colloids.ipynb`](L1_fitting/L1_fitting_colloids.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Edinburgh-Chemistry-Teaching/AdvancedPhysicalChemistry/blob/main/L1_fitting/L1_fitting_colloids.ipynb) | optional |
| L2 | Unsupervised learning | [`L2_unsupervised/L2_unsupervised_wine.ipynb`](L2_unsupervised/L2_unsupervised_wine.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Edinburgh-Chemistry-Teaching/AdvancedPhysicalChemistry/blob/main/L2_unsupervised/L2_unsupervised_wine.ipynb) | optional |
| L3 | Representing chemistry | [`L3_representations/`](L3_representations/) (coming soon) | optional |
| **L4** | **Classification and evaluation ** | [`L4_classification/L4_prework_IR_classification.ipynb`](L4_classification/L4_prework_IR_classification.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Edinburgh-Chemistry-Teaching/AdvancedPhysicalChemistry/blob/main/L4_classification/L4_prework_IR_classification.ipynb) | **required** |
| L5 | Neural networks | [`L5_neural_networks/`](L5_neural_networks/) (coming soon) | optional |

## How to run the notebooks

* **Noteable (recommended):** open the notebook from the lecture page on Learn.
* **Google Colab:** use the *Open in Colab* button. Save a copy to your Drive, or your work will be lost.
* **Locally:** clone the repository, keep the folder structure, and install the packages:

  ```bash
  git clone https://github.com/Edinburgh-Chemistry-Teaching/AdvancedPhysicalChemistry.git
  cd AdvancedPhysicalChemistry
  pip install -r requirements.txt
  jupyter lab
  ```

## Repository layout

```
data/                datasets shared by the notebooks (see data/README.md)
L1_fitting/          Lecture 1 notebook: non-linear fitting of colloid data (optional)
L2_unsupervised/     Lecture 2 notebook (optional)
L3_representations/  Lecture 3 notebook (optional)
L4_classification/   Lecture 4 pre-work notebook (required)
L5_neural_networks/  Lecture 5 notebook (optional)
requirements.txt     Python packages needed
```

## Data and licence

The DLS data for Lecture 1 are simulated. The IR spectra come from the Chemotion Repository, *FT-IR spectroscopy data (Chemotion IR)*, [DOI: 10.22000/OGoEQGlsZGElrgst](https://doi.org/10.22000/OGoEQGlsZGElrgst), CC BY-SA 4.0. Details are in [`data/README.md`](data/README.md).

© Antonia Mey, University of Edinburgh, 2026. This repository uses two licences:

* **Text, notebooks (prose and figures) and data:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), see [`LICENSE`](LICENSE).
* **Code** (the code cells in the notebooks and any `.py` files): [MIT](https://opensource.org/licenses/MIT), see [`LICENSE-CODE`](LICENSE-CODE).

The processed IR data must remain under CC BY-SA 4.0, as required by the original Chemotion licence.
