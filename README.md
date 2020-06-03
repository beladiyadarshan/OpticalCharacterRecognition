# OpticalCharacterRecognition
A classic problem in computer vision recognizing written text through pictures. 

This problem was tackled in two parts:

## 1. [EMNIST Classification](https://github.com/hxt1965/OpticalCharacterRecognition/blob/master/emnist_classification%20.ipynb) 
The [EMNIST dataset](https://www.nist.gov/itl/products-and-services/emnist-dataset) was fed into a Sequential Neural Network consisting of 10 layers, namely, 
 - Conv2D
 - MaxPooling2D
 - Dropout
 - Dense 

The model achieved an accuracy of 85.86%

## 2. [Line Segmentation](https://github.com/hxt1965/OpticalCharacterRecognition/blob/master/Line%20Segmentation.ipynb)
The second part of this project dealt with line segmentation on a given picture with handwritten text. A very primitive approach was taken wherein after converting the image to grayscale, the signal on each horizontal line of text was added up and graphed out. The peaks were identified to be lines and highlighted.
On each highlighted line, the signal on each vertical line of pixels was again added up and the peaks were identified as inidividual characters. The characters were then feeded into the EMNIST model and identified. For each line therefore, each latin character was identified and converted into a UTF-8 readable format. 
