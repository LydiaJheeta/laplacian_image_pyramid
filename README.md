# Laplacian Pyramid Image Compression

Implementation of Gaussian and Laplacian Image Pyramids in Python, based on the classic paper:

> Burt, P. J., & Adelson, E. H. *The Laplacian Pyramid as a Compact Image Code*.

The project was developed as part of an Image and Video Analysis course and implements the complete pyramid construction, reconstruction and quantization pipeline.

---

## Features

- Gaussian kernel generation
- Gaussian Pyramid construction
- Laplacian Pyramid construction
- Image reconstruction from Laplacian Pyramid
- Pyramid quantization
- Entropy analysis
- Support for both grayscale and RGB images

---

## Implemented Algorithms

- Gaussian Kernel
- Gaussian Reduce
- Gaussian Expand
- Gaussian Pyramid
- Laplacian Pyramid
- Pyramid Decoding
- Laplacian Quantization

---

## Experiments

The implementation was evaluated using the classic **Lena** and **Camera** test images.

The following experiments were performed:

- Effect of different kernel parameter values (`a = 0.3 ... 0.7`)
- Effect of pyramid depth (`3–6 levels`)
- Entropy analysis at every pyramid level
- Optimal kernel parameter selection
- Quantization using different bin sizes

---

## Results

### Image Reconstruction

| Original | Reconstructed |
|----------|---------------|
| ✔ | ✔ |

The reconstructed images preserve most visual information while enabling multi-resolution representation.

---

### Entropy Analysis

Entropy was computed for every Laplacian level while varying:

- kernel parameter **a**
- pyramid depth

The experiments identify the parameter values that minimize entropy and improve compression efficiency.

---

### Quantization

Different quantization bin sizes were evaluated to study the trade-off between:

- Compression
- Visual quality
- Information loss

---

## Technologies

- Python
- NumPy
- OpenCV
- Matplotlib
- Jupyter Notebook

---

## Reference

P. Burt and E. Adelson,
**The Laplacian Pyramid as a Compact Image Code**,
IEEE Transactions on Communications, 1983.
