# DCTR

Deep neural networks using Classification for Tuning and Reweighting (DCTR, pronounced “doctor”) is a technique for

 - Reweighting a dataset into another using the full phase-space information (assuming they have support in the same domain)
  - If one of the datasets were generated with a Monte Carlo (MC) generator, DCTR can infer what the optimal MC parameters are for reproducing the other dataset (typically experimental data). This is referred to as MC Tuning.

DCTR was first developed in the context of High Energy Physics, [arXiv:1907.08209](https://arxiv.org/abs/1907.08209), but has applications across physics and possibly beyond.

## Notebooks

We provide a few example notebook to illustrate how DCTR works

### Simple Gaussian Examples
To illustrate the basic idea behind DCTR, we provide
- A basic example just using a Gaussian distribution `./Gaussian-notebooks/GaussianDCTRExample.ipynb`
- Illustration of alternative loss function defined in [Appendix B of arXiv:1907.08209](https://arxiv.org/abs/1907.08209): `./Gaussian-notebooks/AlternativeFit.ipynb`

### High Energy Physics Examples
We provide complete examples of the DCTR code used to generate plots from [arXiv:1907.08209](https://arxiv.org/abs/1907.08209).
There are four notebooks organized based on what MC parameters are changed
- $\texttt{TimeShower:alphaSvalue}$: `./HEP-notebooks/DCTR_1D_alphaS.ipynb`
- $\texttt{StringZ:aLund}$: `./HEP-notebooks/DCTR_1D_aLund.ipynb`
- $\texttt{StringFlav:probStoUD}$: `./HEP-notebooks/DCTR_1D_StoUD.ipynb`
-  All of the above three parameters:  `./HEP-notebooks/DCTR_3D.ipynb`

## Sample Datasets
The datasets used to run the High Energy Physics example notebooks can be found on [Zenodo](https://zenodo.org/record/3518708#.XbN4MJNKjOQ)