# Advanced Physical Chemistry: Machine Learning in Chemistry

Notebooks and data for the six-lecture *Machine Learning in Chemistry* course (Advanced Physical Chemistry, University of Edinburgh, 2026/27).

Lecturer: Dr Antonia Mey (antonia.mey@ed.ac.uk)

## Contents

There is one folder per lecture. Only the Lecture 4 notebook is required; the others are optional extras for practice.

| Lecture | Topic | Notebook | |
|---|---|---|---|
| L1 | From fitting to learning | [`L1_fitting/`](L1_fitting/) (coming soon) | optional |
| L2 | Unsupervised learning | [`L2_unsupervised/L2_unsupervised_wine.ipynb`](L2_unsupervised/L2_unsupervised_wine.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Edinburgh-Chemistry-Teaching/AdvancedPhysicalChemistry/blob/main/L2_unsupervised/L2_unsupervised_wine.ipynb) | optional |
| L3 | Representing chemistry | [`L3_representations/`](L3_representations/) (coming soon) | optional |
| **L4** | **Classification and evaluation (flipped)** | [`L4_classification/L4_prework_IR_classification.ipynb`](L4_classification/L4_prework_IR_classification.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Edinburgh-Chemistry-Teaching/AdvancedPhysicalChemistry/blob/main/L4_classification/L4_prework_IR_classification.ipynb) | **required before Mon 16 Nov** |
| L5 | Neural networks | [`L5_neural_networks/`](L5_neural_networks/) (coming soon) | optional |
| L6 | Frontiers | [`L6_frontiers/`](L6_frontiers/) (coming soon) | optional |

The L4 notebook is the pre-work for the half-flipped lecture: before the lecture, watch the short video, work through Sections 0–5 of the notebook (about 40 minutes) and do the quiz on Learn. Sections 6 and 7 are optional practice after the lecture.

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
L1_fitting/          Lecture 1 notebook (optional)
L2_unsupervised/     Lecture 2 notebook: PCA and k-means on the wine data (optional)
L3_representations/  Lecture 3 notebook (optional)
L4_classification/   Lecture 4 pre-work notebook (required)
L5_neural_networks/  Lecture 5 notebook (optional)
L6_frontiers/        Lecture 6 notebook (optional)
requirements.txt     Python packages needed
```

## Data and licence

The IR spectra come from the Chemotion Repository, *FT-IR spectroscopy data (Chemotion IR)*, [DOI: 10.22000/OGoEQGlsZGElrgst](https://doi.org/10.22000/OGoEQGlsZGElrgst), CC BY-SA 4.0. Details are in [`data/README.md`](data/README.md).

© Antonia Mey, University of Edinburgh, 2026. This repository uses two licences:

* **Text, notebooks (prose and figures) and data:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), see [`LICENSE`](LICENSE).
* **Code** (the code cells in the notebooks and any `.py` files): [MIT](https://opensource.org/licenses/MIT), see [`LICENSE-CODE`](LICENSE-CODE).

The processed IR data must remain under CC BY-SA 4.0, as required by the original Chemotion licence.
