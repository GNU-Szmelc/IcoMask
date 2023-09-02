# IcoMask ~ Modern Icon Toolkit by szmelc

===================================================

## 1.py

### Project Documentation: Image Overlay

**File:** 1.py

**Description:**
This script overlays an image with a transparent image, also known as a mask. It takes user inputs such as the desired overlay, transparency value, and the path to the folder containing the images to be processed. It creates a unique output folder for each process and saves the resulting images with the overlay applied.

#### Files and Purpose:
- `1.py`: It contains the main code for overlaying images with masks. It takes user inputs, processes the images, and saves the output.

#### Usage:
1. Make sure you have installed the required dependencies (see Dependencies section).
2. Place the images you want to overlay in a folder called "png".
3. Place the desired overlay images (masks) in a folder called "mask".
4. Run the script `1.py`.
5. The script will display the available masks in the "mask" folder.
6. Enter the filename of the overlay (mask) you want to use or type "ALL" to process all masks.
7. Enter the transparency value (0-100) for the overlay.
8. The script will create a unique output folder for each process inside the "output" folder.
9. The processed images with the overlay applied will be saved in the respective output folders.

#### File Relationships:
The script interacts with the following files and folders:
- `1.py` interacts with the "png" folder, which contains the images to be processed.
- `1.py` interacts with the "mask" folder, which contains the overlay images (masks).
- `1.py` creates unique output folders within the "output" folder to save the processed images.

#### Dependencies:
This project has the following dependencies:
- PIL (Python Imaging Library)
- os (Built-in Python library)
- datetime (Built-in Python library)

To install the required dependencies, run the following command:
```
pip install pillow
```

#### Notes:
- The transparency value determines the opacity of the overlay. A value of 0 means the overlay is fully opaque, while a value of 100 means the overlay is fully transparent.
- The script processes each image in the "png" folder individually, applying the chosen overlay (mask) to it.
- If you choose "ALL" as the overlay (mask), the script will process all masks available in the "mask" folder.
- The processed images with the overlay applied are saved in unique folders within the "output" folder, named after the chosen overlay and timestamp.

===================================================

## s.py

### Project Documentation: Overlay Images

**File:** s.py

**Description:**
This script is used to overlay images with a chosen mask. It provides functionality to convert SVG images to PNG format, convert raster images to SVG format, and overlay images with transparency.

#### Files and Purpose:
- `s.py`: The main script file that performs the overlay images operation. It includes functions for converting SVG to PNG, raster to SVG, and overlaying images. It also includes a function to process each mask and overlay it on the input images.

#### Usage:
To use this script, follow these steps:
1. Make sure you have the necessary dependencies installed (see Dependencies section below).
2. Place the input images in the "icons" folder.
3. Place the overlay masks (PNG format) in the "mask" folder.
4. Run the script `s.py` using Python.
5. Enter the transparency value (0-100) when prompted.
6. Enter the filename of the overlay (mask) you want to use or type "ALL" to process all available masks.

#### File Relationships:
The `s.py` script interacts with the following files and folders:
- `icons` folder: Contains the input images that need to be overlaid.
- `mask` folder: Contains the overlay masks (PNG format) to be used for overlaying.
- `output` folder: The script creates a unique output folder for each mask and timestamp combination, where the resulting overlay images are saved.

#### Dependencies:
This script requires the following dependencies:
- `os`
- `datetime`
- `PIL` (Python Imaging Library)
- `svgwrite`
- `cairosvg`

Use the following command to install the necessary dependencies using pip:
```
pip install Pillow svgwrite cairosvg
```

#### Notes:
- This script assumes that the input images are in the PNG format and overlay masks are also in the PNG format.
- The resulting overlay images are saved in the respective output folder for each mask and timestamp combination.
- If an input image is in SVG format, it will be converted to PNG first, then overlayed, and finally converted back to SVG before saving.
- The transparency value determines the extent of transparency between the input image and the overlay mask.

===================================================
