# Adobe GenSolve
# Overview
This Jupyter Notebook processes a dataset of coordinates to visualize them and applies image processing techniques to detect and straighten shapes in an image.

Steps:
Load CSV Data and Visualize:

The notebook starts by loading a CSV file that contains coordinate data. The data is plotted on a scatter plot, which is saved as scatter_plot.png.
Shape Detection and Straightening:

The second part of the notebook focuses on image processing using OpenCV.
Contours are detected in the scatter_plot.png image. The notebook then distinguishes between circular and non-circular shapes.
Circular shapes are replaced with perfect circles, and non-circular shapes are straightened to remove irregularities.
Two images are generated: one with the corrected shapes (overdrawn contours) and another where the original shapes are removed.
How to Run
Environment Setup:

Ensure you have the required Python packages installed:
pandas
matplotlib
opencv-python
numpy
Running the Notebook:

Load the notebook in Jupyter or a compatible environment.
Run the cells in order.
The output images will be displayed in the notebook, and scatter_plot.png will be saved to your working directory.
Input Files:

The notebook references a CSV file (frag0.csv) and an image (scatter_plot.png).
Ensure these files are available in the paths specified in the notebook, or update the paths accordingly.
Logic Applied
Scatter Plot Creation: Coordinates from the CSV file are plotted to visualize data points.
Contour Detection: The scatter plot is processed to detect contours, representing shapes in the image.
Shape Correction:
If a shape is circular, it is replaced with a perfect circle.
Other shapes are straightened by approximating their contours to remove irregularities.
