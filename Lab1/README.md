# Lab 1 — Solution Notebook

## Contents
- **Task #2**: load an image with OpenCV (`cv2.imread`) and with PIL (`Image.open`), display both.
- **Task #3**: save an image with OpenCV (`cv2.imwrite`) and with PIL (`.save`).
- **Task #4**: print the image as a NumPy array (shape + values) for both the OpenCV and PIL versions.

## Requirements
- Python packages: `opencv-python`, `pillow`, `matplotlib`, `numpy`
- An `images/` folder next to the notebook containing:
  - `cameraman.tif`
  - `lena_gray_256.tif`

## Notes
- OpenCV loads images in **BGR** order, so colors in `plt.imshow(img)` may look off compared to the original — this is expected with `cv2.imread` + `matplotlib`.
- `lena_gray_256.tif` is a grayscale image, so it's displayed with `cmap=cm.Greys_r`.
