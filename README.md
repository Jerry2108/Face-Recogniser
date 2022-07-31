# Face-Recogniser
# Introduction
1. This is a deep learning project using LBPH classification provided by the openCV library of python to recognize image.
# Installation
Please install these packages if running the file on the local environment: 
1. pip install opencv-python
2. pip install numpy
3. pip install Pillow
# LBPH classification
LBPH uses 4 parameters:

<b>1.Radius</b>: the radius is used to build the circular local binary pattern and represents the radius around the central pixel. It is usually set to 1.

</b>2.Neighbors</b>: the number of sample points to build the circular local binary pattern. Keep in mind: the more sample points you include, the higher the computational cost. It is usually set to 8.

<b>3.Grid X</b>: the number of cells in the horizontal direction. The more cells, the finer the grid, the higher the dimensionality of the resulting feature vector. It is usually set to 8.

<b>4.Grid Y</b>: the number of cells in the vertical direction. The more cells, the finer the grid, the higher the dimensionality of the resulting feature vector. It is usually set to 8.

