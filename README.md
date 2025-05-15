# Parallelized IIkMC for Satellite Images

This project implements and benchmarks **Inter-Image k-Means Clustering (IIkMC)** on large-scale satellite imagery datasets, with support for CPU and memory-efficient parallelization. The approach is designed to scale to multi-scene Landsat data using both full-resolution and downsampled strategies.

Attaching Link as the file is too large to upload:
Dataset Link: https://drive.google.com/drive/folders/1Lya5SiRHvWcn1Hpjs0TKz_tJhVmilF8W?usp=drive_link

---

## 🛰️ Overview

- Cluster large satellite scenes into land-cover classes using a modified k-Means algorithm.
- Supports CPU-parallel execution using `ThreadPoolExecutor`.
- Memory-safe block-wise clustering avoids full Nxk matrix computation.
- Optional downsampling for faster convergence during development.
- Cluster maps visualized using matplotlib with geospatial mask reconstruction.

For more details, refer to "Our research paper".
