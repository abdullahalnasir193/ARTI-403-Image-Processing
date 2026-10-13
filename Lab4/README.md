# ARTI 404 – Image Processing | Lab 4

Intensity transformations and spatial-domain filtering (histogram processing).

## Files
- `Lab4.ipynb` – solutions for the three assessment tasks
- `Lab4_Report.pdf` – report (notebook exported with outputs)
- `images/` – images used (`moon.png`, `rocket.png`, `chelsea.png`, from `skimage.data`)

## Tasks
1. **Contrast stretching** – moon image rescaled to the 3rd–80th percentile range with `exposure.rescale_intensity`, histogram plotted.
2. **Histogram equalization** – `exposure.equalize_hist` on the moon image, image and flattened histogram shown.
3. **Histogram matching** – `exposure.match_histograms` with Chelsea as source and rocket as reference; per-channel histograms compared.

## Requirements
Python 3, NumPy, Matplotlib, scikit-image.
