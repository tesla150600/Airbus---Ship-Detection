# Airbus---Ship-Detection

In this project,need to build a semantic segmentation model using the unet architecture to search for ships on a satellite photo.
The file with weights is big so it is on google drive(https://drive.google.com/drive/folders/1CRn2c3EsGyKGzUTDIpECwf-T_arB8cgE?usp=sharing)

 
The original dataset was taken from Kaggle and uploaded to a laptop from which GPU calculations were performed.
There is an imbalance in the data and most of the photos are without ships at all, so for optimization it is possible to remove most of the photos without ships.


Encode and Decode were taken from this example https://www.kaggle.com/code/paulorzp/run-length-encode-and-decode/script

The initial photos had dimensions of 768x768 and during the work they were compressed to 128x128
 
The training of the Network was carried out on n = 50,000 examples, they were divided into training and validation (75 by 25), as an optimizer I took RMSprop = 0.0001, the binary_crossentropy loss function and the dise score metric.


# Example of network results
![зображення](https://user-images.githubusercontent.com/45979299/186900474-35ce313e-04f5-4871-8bd0-63075d8ffba6.png)

![зображення](https://user-images.githubusercontent.com/45979299/186900735-15f04a44-62ed-491c-8140-bd5f0ead031b.png)

![зображення](https://user-images.githubusercontent.com/45979299/186901129-2946052b-cde8-410b-b4a4-2104c1074d71.png)
