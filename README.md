## knn-spd

#### Article: &nbsp;&nbsp;<small><strong>Metric-Based Supervised Classification of SPD Diffusion Tensor Images</strong> &nbsp;<a href="#"><img src="https://cdn.simpleicons.org/doi/2dd4bf" alt="DOI" height="14" align="absmiddle"></a>&nbsp;&nbsp;<a href="#"><img src="https://cdn.simpleicons.org/zenodo/2dd4bf" alt="Zenodo" height="14" align="absmiddle"></a>&nbsp;&nbsp;<a href="https://drive.google.com/drive/folders/17J6wcAgKmvFCYMCjt43hUQ0ISgCMNDHB?usp=sharing"><img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/google/google-original.svg" alt="Google Drive" height="14" align="absmiddle"></a></small>

We present a computational framework for supervised voxel-wise classification of diffusion tensor MRI (DT-MRI). Each voxel is represented by a 3×3 symmetric positive definite (SPD) matrix, and classification is performed directly on the SPD manifold using *k*-nearest neighbors. The study compares Frobenius (FR), Log-Euclidean (LE), affine-invariant Riemannian (AIRM), and deterministic border–interior hybrid distances under a unified experimental protocol.

The evaluation follows a subject-wise nested design with 20 subjects, five outer folds, subject-wise inner cross-validation for selecting *k*, repeated class-balanced WM/GM/CSF sampling, and paired statistical analysis at the subject level. The repository includes FR, LE, AIRM, H-FR, H-LE, and H-AIRM classifiers together with EUC/FA, LOGREG, LIN-SVM, RBF-SVM, SH-MLP, RF, and RF+GC baselines.

Experiments quantify predictive performance, computational cost, execution time, memory consumption, neighborhood sensitivity, sampling-budget sensitivity, voting strategies, tie frequencies, regional-versus-shared bank construction, erosion-radius sensitivity, and empirical LE–AIRM neighborhood agreement. The study provides a controlled analysis of how metric geometry affects finite-sample neighborhood structure and supervised DT-MRI tensor classification without claiming general superiority over end-to-end segmentation frameworks.

#### Dependencies

- Python >= 3.12
- numpy
- scipy
- scikit-learn
- nibabel
- matplotlib
- psutil

#### Bash

```bash
pip install numpy scipy scikit-learn nibabel matplotlib psutil
```

#### License (MIT)

- Copyright (c) alancampos-ai
- Code released under the MIT License.
