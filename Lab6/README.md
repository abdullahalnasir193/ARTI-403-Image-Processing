# Lab 6 – Frequency Domain

**Course:** ARTI 403 – Image Processing

## Files
- `Lab6.ipynb` – solution notebook
- `Lab6.pdf` – PDF export of the notebook
- `images/` – image used (`cameraman.png`, loaded in the notebook from `skimage.data.camera()`)

## Task
**Sobel filters in the frequency domain** on the Cameraman image (resized to 256x256):
1. Each 3x3 Sobel kernel is zero-padded to the image size, centered, and shifted with `ifftshift` so its origin is at (0,0), then transformed with `fft2` (`center_embed_kernel`).
2. The image FFT is multiplied element-wise with each kernel's FFT.
3. `ifft2` gives the spatial results `Gx` and `Gy`; the gradient magnitude is `sqrt(Gx² + Gy²)`.
4. The original, the filtered spectra, `Gx`, `Gy` and the magnitude are plotted.

## Run
```
pip install numpy matplotlib scikit-image jupyter
jupyter notebook Lab6.ipynb
```
