# Face-Recogniser
# Introduction
1. This is a deep learning project using LBPH classification provided by the openCV library of python to recognize faces. 

2. The model can **recognize** the same face of a person **regardless of any emotion states or whether that person is wearing glasses or not**.

# Installation
Please install these packages if running the file on the local environment: 
1. pip install opencv-python
2. pip install numpy
3. pip install Pillow
**No need to install if running the file directly on Jupyter Notebook.
# LBPH classification
LBPH uses 4 parameters:

<b>1.Radius</b>: the radius is used to build the circular local binary pattern and represents the radius around the central pixel (1 by default).

<b>2.Neighbors</b>: the number of sample points to build the circular local binary pattern. Keep in mind: the more sample points you include, the higher the computational cost (8 by default).

<b>3.Grid X</b>: the number of cells in the horizontal direction. The more cells, the finer the grid, the higher the dimensionality of the resulting feature vector (8 by default).

<b>4.Grid Y</b>: the number of cells in the vertical direction. The more cells, the finer the grid, the higher the dimensionality of the resulting feature vector (8 by default).

We use these 4 parameters to generate a historgram for each image and later on comparing these histograms by statistical methods (Chi Square, Euclidean distance) to recognize faces. 

<img width="773" alt="Screen Shot 2022-07-31 at 10 31 05 pm" src="https://user-images.githubusercontent.com/80389972/182026526-3d37bc79-dccd-4904-865f-1ff764eb6478.png">

More information about the algorithm can be found here: https://towardsdatascience.com/face-recognition-how-lbph-works-90ec258c3d6b

# Result

# # Sample test case:

1. Given this image (this person is wearing glasses): 

![subject01 glasses](https://user-images.githubusercontent.com/80389972/182026724-2a0b9e21-2307-4a17-b8d6-a1c3dbc26688.gif)

2. After being trained, the model can predict the same person: 

![subject01](https://user-images.githubusercontent.com/80389972/182026890-59dafd29-8617-444a-bf5d-0ed7dcb004da.gif)



