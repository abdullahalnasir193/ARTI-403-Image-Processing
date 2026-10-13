# Lab 1 — Solution Notebook

## Contents
- **Task #1**: practice the Python and NumPy cheat sheets in Spyder separately. The referenced cheat sheets are not included in this package.
- **Task #2**: load an image with OpenCV (`cv2.imread`) and with PIL (`Image.open`), display both.
- **Task #3**: save an image with OpenCV (`cv2.imwrite`) and with PIL (`.save`).
- **Task #4**: print the image as a NumPy array (shape + values) for both the OpenCV and PIL versions.

## Requirements
- Python packages: `opencv-python`, `pillow`, `matplotlib`, `numpy`
- An `images/` folder next to the notebook containing:
  - `cameraman.tif`
  - `lena_gray_256.tif`

## Notes
- Run the notebook cells in order, with this folder as the working directory.
- OpenCV loads images in **BGR** order. The notebook converts BGR to RGB for Matplotlib. For the supplied grayscale cameraman image, the three channels are identical, so this conversion does not change its appearance.
- `lena_gray_256.tif` is a grayscale image, displayed with `cmap='gray'` and the intensity range 0–255.
- OpenCV's default read produces a three-dimensional array; Pillow preserves this grayscale image as a two-dimensional array. NumPy abbreviates large arrays when printing.
- Task #3 writes `new_image.jpg` and `new_image2.jpg` in this folder. JPEG is lossy, as in the manual's example.
- The instructions provided here are in `STUDENT PROCEDURAL MANUAL - Lab 1.doc`; no PDF is included.
