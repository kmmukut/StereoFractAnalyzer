
<img align='left' src='https://github.com/kmmukut/StereoFractAnalyzer/assets/32664955/f16ce153-846b-4b9e-8fce-3ecd1809c17a' width = "200" height = "200"> 

[![StereoFractAnalyzer](https://github.com/kmmukut/StereoFractAnalyzer/actions/workflows/StereoFractAnalyzer.yml/badge.svg)](https://github.com/kmmukut/StereoFractAnalyzer/actions/workflows/StereoFractAnalyzer.yml)
[![PyPI version](https://badge.fury.io/py/StereoFractAnalyzer.svg)](https://badge.fury.io/py/StereoFractAnalyzer)

[![Deploy static content to Pages](https://github.com/kmmukut/StereoFractAnalyzer/actions/workflows/static.yml/badge.svg)](https://github.com/kmmukut/StereoFractAnalyzer/actions/workflows/static.yml)

![Version 1.0.0](https://img.shields.io/badge/version-1.0.0-brightgreen)
![Coverage 100%](https://img.shields.io/badge/coverage-100%25-brightgreen) 
![License MIT](https://img.shields.io/badge/license-MIT-green])
[![HitCount](https://hits.dwyl.com/comp-comb/StereoFractAnalyzer.svg?style=flat-square&show=unique)](http://hits.dwyl.com/comp-comb/StereoFractAnalyzer)

Documentation is available at : [https://comp-comb.github.io/StereoFractAnalyzer/](https://comp-comb.github.io/StereoFractAnalyzer/)
---

<!-- ![logo](https://github.com/kmmukut/StereoFractAnalyzer/assets/32664955/165e9dfb-5fd1-438d-863a-71e0158bcccd) -->
<!-- ![logo2](https://github.com/kmmukut/StereoFractAnalyzer/assets/32664955/f16ce153-846b-4b9e-8fce-3ecd1809c17a) -->

# StereoFractAnalyzer



StereoFractAnalyzer is a Python package designed for analyzing the fractal dimension of 3D surfaces and 2D images. It finds applications across various fields such as material science, geology, and computer graphics. Utilizing the capabilities of Open3D, NumPy, Matplotlib, and PIL, it offers a robust suite of tools for comprehensive fractal geometry analysis.

## Features

- **3D Model Analysis**: Load and analyze 3D models from STL files to study their surface complexity.
- **Voxel Grid Conversion**: Convert 3D models into voxel grids to facilitate volumetric analysis.
- **Fractal Dimension Calculation**: Determine the fractal dimension of both 3D surfaces and 2D binary images to quantify their complexity.
- **Visualization Tools**: Utilize visualization capabilities to inspect 3D models, voxel grids, and contour slices of your analytical models.
- **Contour Drawing**: Generate and visualize contours of 3D meshes at specified z-heights, aiding in the understanding of surface features.
- **Surface and Image Complexity Estimation**: Estimate the roughness or complexity of surfaces and images through detailed fractal analysis.

## Installation

Ensure you have Python 3.6 or higher installed on your system. Install StereoFractAnalyzer using pip:

```
pip install StereoFractAnalyzer
```

## Dependencies

StereoFractAnalyzer requires the following libraries:

- open3d
- numpy
- matplotlib
- Pillow

Install these dependencies directly using pip if not already installed:

```
pip install open3d numpy matplotlib Pillow
```

## Usage

### Analyzing a 3D Model

To compute the fractal dimension of a 3D surface:

```python
from StereoFractAnalyzer import StereoFractAnalyzer

analyzer = StereoFractAnalyzer(stl_path="path/to/your/model.stl")
surface_fractal_dimension = analyzer.get_surface_fractal_dimension()
print(f"Surface fractal dimension: {surface_fractal_dimension}")
```

### Analyzing a 2D Image

For fractal dimension analysis of a 2D binary image:

```python
from StereoFractAnalyzer import StereoFractAnalyzer

analyzer = StereoFractAnalyzer(img_path="path/to/your/image.png")
fractal_dimension = analyzer.get_image_fractal_dimension(plot=1)
print(f"The fractal dimension of the image is: {fractal_dimension}")
```

## Command Line Interface

StereoFractAnalyzer's CLI allows for direct terminal-based operations for both 3D and 2D analyses.

### 3D Model Analysis

Analyze a 3D model from an STL file:

```
StereoFractAnalyzer --stl path/to/your/model.stl
```

### 2D Image Analysis

Calculate the fractal dimension of a 2D binary image:

```
StereoFractAnalyzer --img path/to/your/image.png
```

### Combined Analysis

Conduct analyses on both a 3D model and a 2D image in one command:

```
StereoFractAnalyzer --stl path/to/your/model.stl --img path/to/your/image.png
```

### Help and Options

For a detailed list of options and help:

```
StereoFractAnalyzer --help
```

This displays all command-line options available, providing guidance on how to use the CLI effectively.

## Contributing

Contributions are welcome! If you have suggestions for improvements or bug fixes, feel free to fork the repository and submit a pull request.

## License

StereoFractAnalyzer is open-source software licensed under the MIT License. See the LICENSE file for more details.

---
