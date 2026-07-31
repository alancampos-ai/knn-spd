## knn-spd

#### Article:   <small><strong>Metric-Based Supervised Classification of SPD Diffusion Tensor Images</strong>  <a href="#"><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a>  <a href="#"><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a>  <a href="https://drive.google.com/drive/folders/17J6wcAgKmvFCYMCjt43hUQ0ISgCMNDHB?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We present a computational study of supervised voxelwise classification of DT-MRI tensor data. Each voxel is represented by a 3 × 3 symmetric positive-definite (SPD) matrix, and classification is performed directly on SPD(3) using *k*-nearest neighbors. The study compares classifiers based on the Frobenius (FR), Log-Euclidean (LE), and affine-invariant Riemannian (AIRM) metrics, along with deterministic border–interior hybrid variants, under a unified experimental design.

The evaluation includes 20 DT-MRI tensor volumes, five outer folds, inner cross-validation for selecting *k*, repeated class-balanced sampling, and paired statistical analyses across held-out volumes. The repository includes the FR, LE, AIRM, H-FR, H-LE, and H-AIRM classifiers, together with the EUC/FA, LOGREG, LIN-SVM, RBF-SVM, SH-MLP, RF, and RF+GC baselines.

The experiments quantify predictive performance, execution time, memory consumption, sensitivity to neighborhood size and sampling budget, voting strategies, tie frequency, regional versus shared bank construction, sensitivity to the erosion radius, and empirical LE–AIRM neighborhood agreement. The study provides a controlled methodological analysis of how metric geometry affects finite-sample neighborhood structure and supervised classification of DT-MRI tensors.

#### Dependencies

* Python >= 3.12
* numpy
* scipy
* scikit-learn
* nibabel
* matplotlib
* psutil
* torch (optional; required for CUDA)
* PyMaxflow (optional; required for RF+GC)

#### Bash

```bash
pip install numpy scipy scikit-learn nibabel matplotlib psutil
pip install torch
pip install PyMaxflow
```

#### License (MIT)

* Copyright (c) alancampos-ai
* Code released under the MIT License.
