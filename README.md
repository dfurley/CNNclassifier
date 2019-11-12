# CNNclassifier
CNN image classifier for chick embryo stage classification

This repository contains the dataset and code required to train a CNN to classify images of different chick embryo stages (stages 10.1,
10.2, 10.3). 

The dataset is contained in data.zip. When unzipped this contains 2 folders, 'stage10', and 'training_data'. Within 
'training_data' there are subfolders of the 3 catagories the image is trained on (10_1, 10_2, 10_3 - these are the folders that should
be used to get the data in 'cnn2.py'), as well as 'code_test' - a small subset of images which were used to test the rotation and greyscale
programs, and 'raw_data' - containing the orignal images as they were before they had been divided into stages and before any editing was 
done.

'Code' contains the programs used to prepare the data and to train the CNN. The most important program is 'cnn2.py' which is the program 
used to train the CNN. 'Code' also contains the programs used to grayscale and produced the rotated versions of every image ('grayscale.py'
and 'rotate_save.py).

It also contains two .ipynb files which contain the results of the two times I ran trained the CNN, first time using all 3 stages, which 
resulted in an accuracy of around 65% (CNNtest1), and second time using stages 10.1 and 10.3, which resulted in an accuracy of 80% 
(CNNtest2). These results suggest to me that the training is working, as it is more accurate when only differentiating between the two 
stages, and should therefore be investigated further.
