# Gravity Method Tutorial Series
A comprehensive, hands-on computational geophysics tutorial series using Python and Jupyter Notebooks for students, lecturers, and geoscientists.

**Author:** Dicky Ahmad Zaky  
**Affiliation:** Geophysical Engineering Department, Universitas Pertamina  

---

## 📚 Tutorial Overview & Curriculum

This series guides students step-by-step from fundamental potential field physics to advanced 2D mapping and non-linear numerical inversion:

| # | Notebook | Key Topics & Geoscientific Concepts |
|---|---|---|
| **01** | `Tutorial 1 - Forward Modeling Gravity Anomaly.ipynb` | Analytical forward modeling of buried spheres; effect of depth, radius, and density contrast on vertical gravity anomalies ($\Delta g$). |
| **02** | `Tutorial 2 - Spectral Analysis of Gravity Anomaly.ipynb` | 1D Fast Fourier Transform (FFT), wavenumber spectra ($\ln A$ vs $k$), depth estimation via spectral slopes, cut-off wavenumber ($k_c$). |
| **03** | `Tutorial 3 - Gravity Anomaly Separation.ipynb` | Separation of regional-residual gravity fields; Moving Average filter with spectral cut-off window ($N = 2\pi / (k_c \Delta x)$); 1st, 2nd, and 3rd order polynomial trend surface fitting; RMSE benchmarking against synthetic ground truth. |
| **04** | `Tutorial 4 - Gravity Anomaly Mapping.ipynb` | 2D survey grids, Complete Bouguer Anomaly (CBA) contouring, shaded relief / hillshade illumination, edge enhancement filters: First Horizontal Derivative (FHD) and Second Vertical Derivative (SVD) zero-contour fault detection. |
| **05** | `Tutorial 5 - Gravity Inverse Modeling.ipynb` | 1D Non-linear least squares inversion (`scipy.optimize.curve_fit` / TRF algorithm); parameter bounds and uncertainty quantification (covariance matrix); solving non-uniqueness / mass equivalence with density priors. |

---

## 🛠️ Requirements & Installation

The tutorials are designed to run cleanly using standard scientific Python packages:

```bash
pip install numpy scipy matplotlib
```

To run the notebooks:
```bash
jupyter notebook
```

---

## 🎯 Pedagogical Features for Students & Lecturers
* **Self-Contained & Synthetic:** Every notebook generates its own synthetic ground truth dynamically—no external proprietary data files or fragile paths required.
* **Geoscientific Continuity:** Parameters from earlier notebooks (e.g., cutoff wavenumbers from Tutorial 2, sphere geometries from Tutorial 1) carry forward naturally into subsequent tutorials.
* **Guided Exercises:** Each tutorial concludes with reflective conceptual questions and coding exercises designed for classroom assessment or independent study.
