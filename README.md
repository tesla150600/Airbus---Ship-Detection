# Airbus---Ship-Detection

In this project,need to build a semantic segmentation model using the unet architecture to search for ships on a satellite photo.

 
The original dataset was taken from Kaggle and uploaded to a laptop from which GPU calculations were performed.
There is an imbalance in the data and most of the photos are without ships at all, so for optimization it is possible to remove most of the photos without ships.


Encode and Decode were taken from this example https://www.kaggle.com/code/paulorzp/run-length-encode-and-decode/script

The initial photos had dimensions of 768*768 and during the work they were compressed to 128*128
 
The training of the Network was carried out on n = 50,000 examples, they were divided into training and validation (75 by 25), as an optimizer I took RMSprop = 0.0001, the binary_crossentropy loss function and the dise score metric.


