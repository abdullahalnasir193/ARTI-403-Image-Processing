# Lab 5 – Spatial Filtering: Smoothing and Sharpening

**Course:** ARTI 403 – Image Processing

## Files
- `Lab5.ipynb` – solution notebook
- `images/` – images used (`astronaut.png`, `chelsea.png`, `coffee.png`)

## Tasks
1. **7x7 box filter** – the image is convolved with a 7x7 averaging kernel (`np.ones((7,7))/49`) using `cv2.filter2D`. The original and smoothed images are shown side by side.
2. **Gaussian filters** – `cv2.GaussianBlur` is applied with 5x5 and 21x21 kernels. The original and both results are shown side by side. The larger kernel gives much stronger blur.
3. **Laplacian sharpening** – the image is converted to float32, `cv2.Laplacian` with a 3x3 kernel (`ksize=1`) is computed, and the result is sharpened using `np.clip(image_float - laplacian, 0, 1)`. The original, Laplacian and sharpened images are plotted.

## Run
```
pip install opencv-python numpy matplotlib jupyter
jupyter notebook Lab5.ipynb
```
